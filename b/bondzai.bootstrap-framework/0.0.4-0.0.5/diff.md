# Comparing `tmp/bondzai.bootstrap-framework-0.0.4.tar.gz` & `tmp/bondzai.bootstrap-framework-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.bootstrap-framework-0.0.4.tar", last modified: Wed Jun 21 15:39:53 2023, max compression
+gzip compressed data, was "bondzai.bootstrap-framework-0.0.5.tar", last modified: Thu Jun 22 17:12:20 2023, max compression
```

## Comparing `bondzai.bootstrap-framework-0.0.4.tar` & `bondzai.bootstrap-framework-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.627519 bondzai.bootstrap-framework-0.0.4/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-06-21 15:39:53.627664 bondzai.bootstrap-framework-0.0.4/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      141 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.621286 bondzai.bootstrap-framework-0.0.4/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.624837 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/
--rw-r--r--   0 theo       (501) staff       (20)      212 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2696 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/bootstrap.py
--rw-r--r--   0 theo       (501) staff       (20)     9159 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_agent.py
--rw-r--r--   0 theo       (501) staff       (20)    14052 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_com.py
--rw-r--r--   0 theo       (501) staff       (20)     5973 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_config.py
--rw-r--r--   0 theo       (501) staff       (20)     2917 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/file_handler.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/logger.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.627220 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      700 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       52 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      755 2023-06-21 15:39:53.628514 bondzai.bootstrap-framework-0.0.4/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:20.332677 bondzai.bootstrap-framework-0.0.5/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-22 17:12:20.333677 bondzai.bootstrap-framework-0.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      141 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:19.815136 bondzai.bootstrap-framework-0.0.5/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:20.122915 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/
+-rwxrwxrwx   0 root         (0) root         (0)      212 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2696 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/bootstrap.py
+-rwxrwxrwx   0 root         (0) root         (0)     9165 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_agent.py
+-rwxrwxrwx   0 root         (0) root         (0)    14052 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_com.py
+-rwxrwxrwx   0 root         (0) root         (0)     6101 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     2917 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/file_handler.py
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/logger.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:20.306936 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      700 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-22 17:12:18.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-22 17:12:20.337189 bondzai.bootstrap-framework-0.0.5/setup.cfg
```

### Comparing `bondzai.bootstrap-framework-0.0.4/NOTICE` & `bondzai.bootstrap-framework-0.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.4/PKG-INFO` & `bondzai.bootstrap-framework-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/bootstrap.py` & `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_agent.py` & `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,16 @@
             logger.debug("create_dbm_table")
             self.datTable = self.link.create_dbm_table(self.config.get_max_raw_data(),
                                                        self.config.get_max_labels(),
                                                        self.config.get_max_reg_len(),
                                                        self.config.get_max_nb_raw_data()
                                                        )
             logger.debug("create_ctx_table")
-            self.ctxTable = self.link.create_ctx_table(self.config.get_nb_vm())
+
+            self.ctxTable = self.link.create_ctx_table(self.config.get_max_models())
 
             # create special row for correction
             # Row(self.datTable, -1, "lastin")
 
     def register_custom_ops_in_agent(self,custom_ops):
         for op in custom_ops:
             self.config.register_external_ops(op,custom_ops[op])
```

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_com.py` & `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_com.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_config.py` & `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,18 @@
                         all_axis.append(model["description"]["axis"])
                         self.max_labels +=1
                 else:
                     reg_len = model["deeplomath"]["mode"]["dim_out"]
                     if reg_len > self.max_reg_len:
                         self.max_reg_len = reg_len
 
-                self.max_models += model["description"]["maxsplit"]
+                if model["description"]["maxsplit"] == 0:
+                    self.max_models +=1    
+                else:
+                    self.max_models += model["description"]["maxsplit"]
 
             bootstrap_info = vm.get_bootstrap_info()
             if bootstrap_info is not None :
                 self.bootstrap_info[vm.get_name()] =  bootstrap_info
                 if "source" in bootstrap_info:
                     if self.max_raw_data < bootstrap_info["source"]["preproc_out_len"] :
                         self.max_raw_data = bootstrap_info["source"]["preproc_out_len"]
```

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/file_handler.py` & `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/file_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/PKG-INFO` & `bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/SOURCES.txt` & `bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.4/setup.cfg` & `bondzai.bootstrap-framework-0.0.5/setup.cfg`

 * *Files identical despite different names*

