# Comparing `tmp/hcai-nova-utils-0.7.0.tar.gz` & `tmp/hcai-nova-utils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-utils-0.7.0.tar", last modified: Mon Jun 19 13:00:33 2023, max compression
+gzip compressed data, was "hcai-nova-utils-0.7.1.tar", last modified: Thu Jun 22 07:31:50 2023, max compression
```

## Comparing `hcai-nova-utils-0.7.0.tar` & `hcai-nova-utils-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.933400 hcai-nova-utils-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-19 13:00:33.933400 hcai-nova-utils-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.929400 hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-19 13:00:33.000000 hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-19 13:00:33.000000 hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 13:00:33.000000 hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-19 13:00:33.000000 hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-19 13:00:33.000000 hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.929400 hcai-nova-utils-0.7.0/nova_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.929400 hcai-nova-utils-0.7.0/nova_utils/db_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/db_utils/nova_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.929400 hcai-nova-utils-0.7.0/nova_utils/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/interfaces/dataset_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/interfaces/server_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.933400 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7930 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_xml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:33.933400 hcai-nova-utils-0.7.0/nova_utils/storage_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/storage_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/nova_utils/storage_utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 13:00:33.933400 hcai-nova-utils-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-06-19 13:00:21.000000 hcai-nova-utils-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/db_utils/nova_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/interfaces/dataset_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/interfaces/server_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7930 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_sample_list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_xml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/storage_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/storage_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/storage_utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/setup.py
```

### Comparing `hcai-nova-utils-0.7.0/PKG-INFO` & `hcai-nova-utils-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.7.0
+Version: 0.7.1
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/PKG-INFO` & `hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.7.0
+Version: 0.7.1
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.7.0/hcai_nova_utils.egg-info/SOURCES.txt` & `hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/db_utils/nova_types.py` & `hcai-nova-utils-0.7.1/nova_utils/db_utils/nova_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/interfaces/dataset_iterable.py` & `hcai-nova-utils-0.7.1/nova_utils/interfaces/dataset_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/interfaces/server_module.py` & `hcai-nova-utils-0.7.1/nova_utils/interfaces/server_module.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_anno_utils.py` & `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_data_types.py` & `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_data_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_sample_list_utils.py` & `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_sample_list_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_stream_utils.py` & `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_stream_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/ssi_utils/ssi_xml_utils.py` & `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_xml_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.0/nova_utils/storage_utils/cache.py` & `hcai-nova-utils-0.7.1/nova_utils/storage_utils/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 def retreive_from_url(url, fp):
 
     with requests.get(url, stream=True, headers={'Accept-Encoding': None}) as r:
 
         # check header to get content length, in bytes
-        total_length = int(r.headers.get("Content-Length"))
+        total_length = int(r.headers.get("Content-Length"),0)
 
         # implement progress bar via tqdm
         with tqdm.wrapattr(r.raw, "read", total=total_length, desc="")as raw:
 
             # save the output to a file
             with open(fp, 'wb')as output:
                 shutil.copyfileobj(raw, output)
@@ -30,8 +30,11 @@
 
     if tmp_file.is_file():
         print(f'File {tmp_file} already exists. Skipping download.')
     else:
         retreive_from_url(url, tmp_file)
 
     with ZipFile(tmp_file) as zObject:
-        zObject.extractall(path=Path(extract_to))
+        zObject.extractall(path=Path(extract_to))
+
+if __name__ == '__main__':
+    retreive_from_url("https://github.com/saveli/syncpy/archive/refs/heads/master.zip",'blub.zip')
```

### Comparing `hcai-nova-utils-0.7.0/setup.py` & `hcai-nova-utils-0.7.1/setup.py`

 * *Files identical despite different names*

