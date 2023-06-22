# Comparing `tmp/remotivelabs_cli-0.0.1a6.tar.gz` & `tmp/remotivelabs_cli-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a6.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a7.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a6.tar` & `remotivelabs_cli-0.0.1a7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a6/LICENSE
--rw-r--r--   0        0        0     2095 2023-06-22 08:12:57.643193 remotivelabs_cli-0.0.1a6/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a6/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a6/cli/__init__.py
--rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a6/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a6/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3538 2023-06-22 08:03:29.813439 remotivelabs_cli-0.0.1a6/cli/cloud/auth.py
--rw-r--r--   0        0        0     2940 2023-06-22 08:03:46.314372 remotivelabs_cli-0.0.1a6/cli/cloud/auth_keys.py
--rw-r--r--   0        0        0     2323 2023-06-22 08:07:25.218764 remotivelabs_cli-0.0.1a6/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1580 2023-06-21 13:16:22.379502 remotivelabs_cli-0.0.1a6/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a6/cli/cloud/configs.py
--rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a6/cli/cloud/projects.py
--rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a6/cli/cloud/recordings.py
--rw-r--r--   0        0        0     3486 2023-06-21 12:56:24.052615 remotivelabs_cli-0.0.1a6/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a6/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a6/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a6/cli/lib/__about__.py
--rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a6/cli/lib/broker.py
--rw-r--r--   0        0        0      432 2023-06-22 08:58:34.023633 remotivelabs_cli-0.0.1a6/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a6/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a6/cli/test/test_simple.py
--rw-r--r--   0        0        0      498 2023-06-22 09:00:33.296453 remotivelabs_cli-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a7/LICENSE
+-rw-r--r--   0        0        0     2095 2023-06-22 08:12:57.643193 remotivelabs_cli-0.0.1a7/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a7/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a7/cli/__init__.py
+-rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a7/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a7/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-22 08:03:29.813439 remotivelabs_cli-0.0.1a7/cli/cloud/auth.py
+-rw-r--r--   0        0        0     2940 2023-06-22 08:03:46.314372 remotivelabs_cli-0.0.1a7/cli/cloud/auth_keys.py
+-rw-r--r--   0        0        0     2323 2023-06-22 08:07:25.218764 remotivelabs_cli-0.0.1a7/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1580 2023-06-21 13:16:22.379502 remotivelabs_cli-0.0.1a7/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a7/cli/cloud/configs.py
+-rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a7/cli/cloud/projects.py
+-rw-r--r--   0        0        0     7899 2023-06-22 15:52:20.798411 remotivelabs_cli-0.0.1a7/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     3486 2023-06-21 12:56:24.052615 remotivelabs_cli-0.0.1a7/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a7/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a7/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a7/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a7/cli/lib/broker.py
+-rw-r--r--   0        0        0      432 2023-06-22 08:58:34.023633 remotivelabs_cli-0.0.1a7/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a7/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a7/cli/test/test_simple.py
+-rw-r--r--   0        0        0      498 2023-06-22 16:21:19.512051 remotivelabs_cli-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a7/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a6/LICENSE` & `remotivelabs_cli-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/README.md` & `remotivelabs_cli-0.0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/brokers.py` & `remotivelabs_cli-0.0.1a7/cli/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/auth_keys.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/auth_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/cloud_cli.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/projects.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/projects.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/recordings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import signal
+import re
 from multiprocessing import Process
 import typer
 import requests
 import os
 import json
 import shutil
 from rich.progress import Progress, SpinnerColumn, TextColumn
@@ -158,7 +159,34 @@
         if r.status_code == 200:
             headers = {}
             headers["content-type"] = "application/x-www-form-urlencoded"
             r = requests.put(r.text, open(file, 'rb'), headers = headers)
             print("File successfully uploaded, please run 'remotive cloud recordings list' to verify that the recording was successfully processed")
         else:
             print(r.text)
+
+@app.command()
+def download_config(
+        recording_session: str = typer.Option(..., help="Recording session id"),
+        broker_config_name: str = typer.Option(..., help="Broker config name"),
+        project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')
+):
+    rest.ensure_auth_token()
+    #print(rest.base_url)
+    r = rest.handle_get(url=f"/api/project/{project}/files/recording/{recording_session}/configuration/{broker_config_name}", return_response=True)
+    #print(r.status_code)
+    #print(r.headers)
+    #print(get_filename_from_cd(r.headers.get('content-disposition')))
+    filename=get_filename_from_cd(r.headers.get('content-disposition'))
+    open(filename, 'wb').write(r.content)
+    print(f'Downloaded file {filename}')
+
+def get_filename_from_cd(cd):
+    """
+    Get filename from content-disposition
+    """
+    if not cd:
+        return None
+    fname = re.findall('filename=(.+)', cd)
+    if len(fname) == 0:
+        return None
+    return fname[0]
```

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/rest_helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/service_account_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.1a7/cli/cloud/service_accounts.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a7/cli/lib/broker.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a6/PKG-INFO` & `remotivelabs_cli-0.0.1a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: 
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

