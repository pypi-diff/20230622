# Comparing `tmp/tttpquisby-0.0.5.tar.gz` & `tmp/tttpquisby-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tttpquisby-0.0.5.tar", last modified: Mon Jun 19 14:18:43 2023, max compression
+gzip compressed data, was "tttpquisby-0.0.6.tar", last modified: Thu Jun 22 10:29:48 2023, max compression
```

## Comparing `tttpquisby-0.0.5.tar` & `tttpquisby-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-13 14:39:53.000000 tttpquisby-0.0.5/LICENSE
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/MANIFEST.in
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1268 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/PKG-INFO
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/README.md
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/requirements.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/setup.cfg
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      953 2023-06-19 14:18:42.000000 tttpquisby-0.0.5/setup.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.217933 tttpquisby-0.0.5/src/
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.218933 tttpquisby-0.0.5/src/pquisby/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.218933 tttpquisby-0.0.5/src/pquisby/command/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/compare_benchmark.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/main.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/command/process_benchmark.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.219933 tttpquisby-0.0.5/src/pquisby/lib/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.219933 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.220933 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/comparison.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/graph.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5326 2023-06-13 15:02:10.000000 tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/uperf.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/compare_sheets.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.220933 tttpquisby-0.0.5/src/pquisby/lib/credentials/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/credentials/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/credentials/creds.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2382 2023-06-19 14:14:22.000000 tttpquisby-0.0.5/src/pquisby/lib/post_processing.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.221933 tttpquisby-0.0.5/src/pquisby/lib/pricing/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/pricing/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/pricing/cloud_pricing.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/process_result.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.221933 tttpquisby-0.0.5/src/pquisby/lib/sheet/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/sheet/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/sheet/sheet_util.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/sheet/sheetapi.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-13 14:40:39.000000 tttpquisby-0.0.5/src/pquisby/lib/util.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-19 14:18:43.222933 tttpquisby-0.0.5/src/tttpquisby.egg-info/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1268 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/PKG-INFO
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1079 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/SOURCES.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/dependency_links.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/entry_points.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/requires.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-19 14:18:43.000000 tttpquisby-0.0.5/src/tttpquisby.egg-info/top_level.txt
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.940943 tttpquisby-0.0.6/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-13 14:39:53.000000 tttpquisby-0.0.6/LICENSE
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/MANIFEST.in
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1268 2023-06-22 10:29:48.940943 tttpquisby-0.0.6/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/README.md
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/requirements.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-22 10:29:48.940943 tttpquisby-0.0.6/setup.cfg
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      953 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/setup.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.936943 tttpquisby-0.0.6/src/
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.937943 tttpquisby-0.0.6/src/pquisby/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.937943 tttpquisby-0.0.6/src/pquisby/command/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/command/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/command/compare_benchmark.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/command/main.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/command/process_benchmark.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.938943 tttpquisby-0.0.6/src/pquisby/lib/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.938943 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.938943 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/comparison.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/graph.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5430 2023-06-22 10:27:11.000000 tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/uperf.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/compare_sheets.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.938943 tttpquisby-0.0.6/src/pquisby/lib/credentials/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/credentials/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/credentials/creds.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2503 2023-06-22 10:27:11.000000 tttpquisby-0.0.6/src/pquisby/lib/post_processing.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.939942 tttpquisby-0.0.6/src/pquisby/lib/pricing/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/pricing/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/pricing/cloud_pricing.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/process_result.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.939942 tttpquisby-0.0.6/src/pquisby/lib/sheet/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/sheet/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/sheet/sheet_util.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/sheet/sheetapi.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-13 14:40:39.000000 tttpquisby-0.0.6/src/pquisby/lib/util.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 10:29:48.939942 tttpquisby-0.0.6/src/tttpquisby.egg-info/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1268 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/src/tttpquisby.egg-info/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1079 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/src/tttpquisby.egg-info/SOURCES.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/src/tttpquisby.egg-info/dependency_links.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/src/tttpquisby.egg-info/entry_points.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/src/tttpquisby.egg-info/requires.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-22 10:29:48.000000 tttpquisby-0.0.6/src/tttpquisby.egg-info/top_level.txt
```

### Comparing `tttpquisby-0.0.5/LICENSE` & `tttpquisby-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/PKG-INFO` & `tttpquisby-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tttpquisby
-Version: 0.0.5
+Version: 0.0.6
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tttpquisby-0.0.5/README.md` & `tttpquisby-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/requirements.txt` & `tttpquisby-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/setup.py` & `tttpquisby-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = (HERE / "README.md").read_text()
 
 # The text of the README file
 REQUIRE = (HERE / "requirements.txt").read_text()
 
 setup(
     name="tttpquisby",
-    version="0.0.5",
+    version="0.0.6",
     description="Quisby is a data processing and visualization tool for benchmark testing.",
     url = 'https://github.com/sousinha1997/Quisby',
     author = 'Soumya Sinha',
     author_email = 'sinhasoumya97@gmail.com',
     license = 'GPL v3.0',
     packages=find_packages("src"),
     package_dir={"":"src"},
```

### Comparing `tttpquisby-0.0.5/src/pquisby/command/process_benchmark.py` & `tttpquisby-0.0.6/src/pquisby/command/process_benchmark.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/comparison.py` & `tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/comparison.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/graph.py` & `tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/graph.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/benchmarks/uperf/uperf.py` & `tttpquisby-0.0.6/src/pquisby/lib/benchmarks/uperf/uperf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     return summary_results
 
 
 def extract_uperf_data(dataset_name, csv_data):
     """"""
     results = []
     data_position = {}
-    results_json = {"data": []}
+    results_json = {"dataset_name": "", "data": []}
     tests_supported = ["tcp_stream", "tcp_rr", "tcp_bidirec", "tcp_maerts"]
 
     for index, row in enumerate(csv_data[0]):
         if "all" in row:
             data_position[row.split(":")[0]] = index
     filtered_result = []
     # Keep only required test results
@@ -85,34 +85,35 @@
                 if item[data_position[key]]:
                     if key in data_dict:
                         data_dict[key].append(
                             [instance_count, item[data_position[key]]]
                         )
                     else:
                         data_dict[key] = [[instance_count, item[data_position[key]]]]
-        test_json = {
-            "vm_name": "",
-            "test_name": "",
-            "metrics_unit": "",
-            "instances": [],
-        }
+
         for key, test_results in data_dict.items():
+            test_json = {
+                "vm_name": "",
+                "test_name": "",
+                "metrics_unit": "",
+                "instances": [],
+            }
             if test_results:
-                test_json["dataset_name"] = dataset_name
                 test_json["test_name"] = "".join(test_name)
                 test_json["metrics_unit"] = key
                 results.append([""])
                 results.append(["".join(test_name)])
                 results.append(["Instance Count", key])
                 for instance_count, items in groupby(
                     test_results, key=lambda x: x[0].split("-")[0]
                 ):
                     items = list(items)
                     item_json = {}
                     item_json["name"] = instance_count
+                    item_json["dataset_name"] = dataset_name
                     if len(items) > 1:
                         failed_run = True
                         for item in items:
                             if "fail" not in item[0]:
                                 item_json["status"] = "pass"
                                 item_json["time_taken"] = item[0]
                                 test_json["instances"].append(item_json)
@@ -125,16 +126,16 @@
                             test_json["instances"].append(item_json)
                             results.append([instance_count, "fail"])
                     else:
                         item_json["status"] = "pass"
                         item_json["time_taken"] = items[0][1]
                         test_json["instances"].append(item_json)
                         results.append(*items)
-        results_json["data"].append(test_json)
-
+            results_json["data"].append(test_json)
+        results_json["dataset_name"] = dataset_name
     return results, results_json
 
 
 if __name__ == "__main__":
     print(
         extract_uperf_data(
             "localhost",
```

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/compare_sheets.py` & `tttpquisby-0.0.6/src/pquisby/lib/compare_sheets.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/credentials/creds.py` & `tttpquisby-0.0.6/src/pquisby/lib/credentials/creds.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/post_processing.py` & `tttpquisby-0.0.6/src/pquisby/lib/post_processing.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     UPERF = enum.auto()
     FIO = enum.auto()
     LINPACK = enum.auto()
     SPECJBB = enum.auto()
 
 
 class QuisbyProcessing:
-    def quisby_extract_data(self, test_name, dataset_name, input_type, data):
+    def extract_data(self, test_name, dataset_name, input_type, data):
         try:
             if input_type == InputType.STREAM:
                 csv_data = stream_to_csv(data)
             elif input_type == InputType.CSV:
                 csv_data = data
             elif input_type == InputType.OTHER_FILE:
                 with open(data) as csv_file:
@@ -44,19 +44,19 @@
                 "exception": str(exc),
                 "exception_type": exception_type,
             }
         return {"status": "success", "csv_data": ret_val, "json_data": json_data}
 
     def compare_csv_to_json(self, benchmark_name, input_type, data_stream):
         result_json = {}
+        comp_dataset_name = "result"
         flag = 0
         for dataset_name, data in data_stream.items():
-            json_res = self.quisby_extract_data(
-                benchmark_name, dataset_name, input_type, data
-            )
+            comp_dataset_name = comp_dataset_name + "_" + dataset_name
+            json_res = self.extract_data(benchmark_name, dataset_name, input_type, data)
             if json_res["json_data"]:
                 json_data = json_res["json_data"]
             if flag == 0:
                 result_json = json_data
                 flag = flag + 1
             else:
                 for i in result_json["data"]:
@@ -64,8 +64,10 @@
                     test_name = i["test_name"]
                     for j in json_data["data"]:
                         if (
                             metric_unit == j["metrics_unit"]
                             and test_name == j["test_name"]
                         ):
                             i["instances"].extend(j["instances"])
+        result_json["dataset_name"] = comp_dataset_name
         return result_json
+
```

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/pricing/cloud_pricing.py` & `tttpquisby-0.0.6/src/pquisby/lib/pricing/cloud_pricing.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/process_result.py` & `tttpquisby-0.0.6/src/pquisby/lib/process_result.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/sheet/sheet_util.py` & `tttpquisby-0.0.6/src/pquisby/lib/sheet/sheet_util.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/sheet/sheetapi.py` & `tttpquisby-0.0.6/src/pquisby/lib/sheet/sheetapi.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/pquisby/lib/util.py` & `tttpquisby-0.0.6/src/pquisby/lib/util.py`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/tttpquisby.egg-info/PKG-INFO` & `tttpquisby-0.0.6/src/tttpquisby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tttpquisby
-Version: 0.0.5
+Version: 0.0.6
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tttpquisby-0.0.5/src/tttpquisby.egg-info/SOURCES.txt` & `tttpquisby-0.0.6/src/tttpquisby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tttpquisby-0.0.5/src/tttpquisby.egg-info/requires.txt` & `tttpquisby-0.0.6/src/tttpquisby.egg-info/requires.txt`

 * *Files identical despite different names*

