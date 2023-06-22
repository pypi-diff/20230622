# Comparing `tmp/stig_edit-1.0.5.tar.gz` & `tmp/stig_edit-1.0.6.tar.gz`

## Comparing `stig_edit-1.0.5.tar` & `stig_edit-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.pylintrc
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.github/workflows/merge.yml
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stig_edit-1.0.5/stig_edit/__init__.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 stig_edit-1.0.5/stig_edit/ckl_editor.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 stig_edit-1.0.5/stig_edit/handler.py
--rw-r--r--   0        0        0  2134120 2020-02-02 00:00:00.000000 stig_edit-1.0.5/tests/test.ckl
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 stig_edit-1.0.5/tests/test_stig_edit.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stig_edit-1.0.5/LICENSE
--rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 stig_edit-1.0.5/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 stig_edit-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 stig_edit-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 stig_edit-1.0.6/.pylintrc
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 stig_edit-1.0.6/.github/workflows/merge.yml
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 stig_edit-1.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stig_edit-1.0.6/stig_edit/__init__.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 stig_edit-1.0.6/stig_edit/ckl_editor.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 stig_edit-1.0.6/stig_edit/handler.py
+-rw-r--r--   0        0        0  2134120 2020-02-02 00:00:00.000000 stig_edit-1.0.6/tests/test.ckl
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 stig_edit-1.0.6/tests/test_stig_edit.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 stig_edit-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stig_edit-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 stig_edit-1.0.6/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 stig_edit-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6284 2020-02-02 00:00:00.000000 stig_edit-1.0.6/PKG-INFO
```

### Comparing `stig_edit-1.0.5/.pylintrc` & `stig_edit-1.0.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/.github/workflows/merge.yml` & `stig_edit-1.0.6/.github/workflows/merge.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 name: Test and publish python package to PyPi
 on:
   pull_request:
     branches: [main]
     types: [closed]
+  push:
+    branches: [main]
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
```

### Comparing `stig_edit-1.0.5/.github/workflows/test.yml` & `stig_edit-1.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/stig_edit/ckl_editor.py` & `stig_edit-1.0.6/stig_edit/ckl_editor.py`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/stig_edit/handler.py` & `stig_edit-1.0.6/stig_edit/handler.py`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/tests/test.ckl` & `stig_edit-1.0.6/tests/test.ckl`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/tests/test_stig_edit.py` & `stig_edit-1.0.6/tests/test_stig_edit.py`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/LICENSE` & `stig_edit-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stig_edit-1.0.5/README.md` & `stig_edit-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 import ckl_editor
 print(ckl_editor.read_target_data("test.ckl"))
 ```
     
 
 ---
 
-### **write_target_data**(*file_name*, *key*, *value*, *target_list*)
+### **write_target_data**(*file_name*, *key*, *value*)
 
 This module can write to any of the Target Data fields shown in the *Editable Fields/Target Data* section. Note the values because some fields must match a list of predefined values or the STIG Viewer will not be able to open the file.
 
 Before running this module, you need to run the *load_target_data()* module and use that as the input for target_list. 
 
 | Parameters        | Description                                               | Examples         | Required |
 |:------------------|:----------------------------------------------------------|:-----------------|:---------|
@@ -72,15 +72,15 @@
 import ckl_editor
 
 ckl_editor.write_target_data(file_name="test.ckl", key="ROLE", value="Member Server")
 ```
 
 ---
 
-### **write_vkey_data**(*file_name*, *key*, *status*, *finding_details*, *comments*, *vkeylist*)
+### **write_vkey_data**(*file_name*, *key*, *status*, *finding_details*, *comments*)
 
 This module can write status, finding_details, and comments to any vkey that exists in your CKL file. It will error out if the vkey does not exists. Some of the fileds such as status have a list of predefined values you must use or the STIG Viewer will not be able to open the file.
 
 Before running this module, you need to run the *load_vkey_data()* module and use that as the input for vkeylist.
 
 | Parameters        | Description                                            | Examples         | Required |
 |:------------------|:-------------------------------------------------------|:-----------------|:---------|
```

### Comparing `stig_edit-1.0.5/pyproject.toml` & `stig_edit-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stig_edit"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="fourhole", email="fourhole7@gmail.com" },
 ]
 description = "A small package that allows you to easily edit STIG (CKL files) quickly."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `stig_edit-1.0.5/PKG-INFO` & `stig_edit-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stig_edit
-Version: 1.0.5
+Version: 1.0.6
 Summary: A small package that allows you to easily edit STIG (CKL files) quickly.
 Project-URL: Homepage, https://github.com/FourHole/stig_edit
 Project-URL: Bug Tracker, https://github.com/FourHole/stig_edit/issues
 Author-email: fourhole <fourhole7@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 import ckl_editor
 print(ckl_editor.read_target_data("test.ckl"))
 ```
     
 
 ---
 
-### **write_target_data**(*file_name*, *key*, *value*, *target_list*)
+### **write_target_data**(*file_name*, *key*, *value*)
 
 This module can write to any of the Target Data fields shown in the *Editable Fields/Target Data* section. Note the values because some fields must match a list of predefined values or the STIG Viewer will not be able to open the file.
 
 Before running this module, you need to run the *load_target_data()* module and use that as the input for target_list. 
 
 | Parameters        | Description                                               | Examples         | Required |
 |:------------------|:----------------------------------------------------------|:-----------------|:---------|
@@ -86,15 +86,15 @@
 import ckl_editor
 
 ckl_editor.write_target_data(file_name="test.ckl", key="ROLE", value="Member Server")
 ```
 
 ---
 
-### **write_vkey_data**(*file_name*, *key*, *status*, *finding_details*, *comments*, *vkeylist*)
+### **write_vkey_data**(*file_name*, *key*, *status*, *finding_details*, *comments*)
 
 This module can write status, finding_details, and comments to any vkey that exists in your CKL file. It will error out if the vkey does not exists. Some of the fileds such as status have a list of predefined values you must use or the STIG Viewer will not be able to open the file.
 
 Before running this module, you need to run the *load_vkey_data()* module and use that as the input for vkeylist.
 
 | Parameters        | Description                                            | Examples         | Required |
 |:------------------|:-------------------------------------------------------|:-----------------|:---------|
```

