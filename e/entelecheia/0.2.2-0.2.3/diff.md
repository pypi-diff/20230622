# Comparing `tmp/entelecheia-0.2.2.tar.gz` & `tmp/entelecheia-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.2.2.tar", max compression
+gzip compressed data, was "entelecheia-0.2.3.tar", max compression
```

## Comparing `entelecheia-0.2.2.tar` & `entelecheia-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-06-14 20:03:44.316047 entelecheia-0.2.2/LICENSE
--rw-r--r--   0        0        0     1591 2023-06-14 20:03:44.316047 entelecheia-0.2.2/README.md
--rw-r--r--   0        0        0     3064 2023-06-14 20:04:11.980383 entelecheia-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      292 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      379 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-06-14 20:04:11.920383 entelecheia-0.2.2/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      353 2023-06-14 20:04:11.920383 entelecheia-0.2.2/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      167 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/copier/conf.yaml
--rw-r--r--   0        0        0      701 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      717 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0      123 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      554 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1518 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      669 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-14 20:03:44.320047 entelecheia-0.2.2/src/entelecheia/py.typed
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 entelecheia-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-21 23:52:11.549439 entelecheia-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1591 2023-06-21 23:52:11.549439 entelecheia-0.2.3/README.md
+-rw-r--r--   0        0        0     3065 2023-06-21 23:52:35.897289 entelecheia-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-06-21 23:52:11.549439 entelecheia-0.2.3/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      379 2023-06-21 23:52:11.549439 entelecheia-0.2.3/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-21 23:52:35.845286 entelecheia-0.2.3/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      353 2023-06-21 23:52:35.845286 entelecheia-0.2.3/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      167 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0       83 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      554 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      396 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/path/__task__.yaml
+-rw-r--r--   0        0        0       85 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/pipe/__external__.yaml
+-rw-r--r--   0        0        0      113 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       51 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/pipe/__instance__.yaml
+-rw-r--r--   0        0        0       49 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/pipe/__lambda__.yaml
+-rw-r--r--   0        0        0      806 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      153 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      195 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/conf/task/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 23:52:11.553439 entelecheia-0.2.3/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 entelecheia-0.2.3/PKG-INFO
```

### Comparing `entelecheia-0.2.2/LICENSE` & `entelecheia-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.2/README.md` & `entelecheia-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.2/pyproject.toml` & `entelecheia-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.2.2"
+version = "0.2.3"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 repository = "https://github.com/entelecheia/entelecheia"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
 
 [tool.poetry.scripts]
 entelecheia = 'entelecheia.__cli__:main'
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.5.1"
+hyfi = "^0.12.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/copier/conf.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/copier/conf.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Source path where to find the template.
 src_path: conf
 # Destination path where to render the template.
-dst_path: .
+dst_path: tmp/conf
 # Filetypes to copy.
 filetypes:
   - yaml
   - yml
   - py
 # User-chosen additional file exclusion patterns.
 exclude:
```

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 DOTENV_FILENAME: .env
 DOTENV_DIR: ${oc.select:..path.runtime,.}
 DOTENV_PATH: ${.DOTENV_DIR}/${.DOTENV_FILENAME}
 # Internal
 HYFI_RESOURCE_DIR:
-HYFI_GLOBAL_WORKSPACE_ROOT:
-HYFI_GLOBAL_DATA_ROOT:
+HYFI_GLOBAL_ROOT:
+HYFI_GLOBAL_WORKSPACE_NAME:
 HYFI_PROJECT_NAME:
 HYFI_TASK_NAME:
+HYFI_PROJECT_DESC:
 HYFI_PROJECT_ROOT:
-HYFI_PROJECT_DATA_ROOT:
+HYFI_PROJECT_WORKSPACE_NAME:
 HYFI_LOG_LEVEL: WARNING
 HYFI_VERBOSE: false
-NUM_WORKERS:
+HYFI_NUM_WORKERS:
 CACHED_PATH_CACHE_ROOT:
 # For other packages
 CUDA_DEVICE_ORDER:
 CUDA_VISIBLE_DEVICES:
 WANDB_PROJECT:
 WANDB_DISABLED:
 WANDB_DIR:
```

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/mode/__init__.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # @package _global_
 debug_mode: false
 print_config: false
-print_resolved_config: true
+resolve: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
+hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
 
 hydra:
   job:
-    name: ${project.project_name}
+    name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
     chdir: true
   run:
-    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${hydra_log_dir}/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
-    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${hydra_log_dir}/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
   job_logging:
     handlers:
       console:
         level: ${hydra.job_logging.root.level}
       file:
         level: ${hydra.job_logging.root.level}
     root:
-      level: ${oc.env:HYFI_LOG_LEVEL,INFO}
+      level: ${logging_level}
```

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/path/__init__.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 # This file defines the path variables used in the project.
 # internal paths for hyfi
 home: ${__home_path__:}
 hyfi: ${__hyfi_path__:}
 resources: ${alt:${oc.env:HYFI_RESOURCE_DIR,null},${.hyfi}/resources}
 runtime: ${get_original_cwd:}
 # global paths
-global_workspace_root: ${oc.select:..global_workspace_root,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_ROOT,null},${__home_path__:}/.hyfi}}
-global_data_root: ${oc.select:..global_data_root,${alt:${oc.env:HYFI_GLOBAL_DATA_ROOT,null},${.global_workspace_root}/data}}
-global_archive: ${.global_data_root}/archive
-global_datasets: ${.global_data_root}/datasets
-global_models: ${.global_data_root}/models
-global_modules: ${.global_data_root}/modules
-global_library: ${.global_data_root}/libs
-global_logs: ${.global_data_root}/logs
+global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}
+global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}
+global_workspace_root: ${.global_hyfi_root}/${.global_workspace_name}
+global_archive: ${.global_workspace_root}/archive
+global_datasets: ${.global_workspace_root}/datasets
+global_models: ${.global_workspace_root}/models
+global_modules: ${.global_workspace_root}/modules
+global_library: ${.global_workspace_root}/libs
+global_logs: ${.global_workspace_root}/logs
 global_cache: ${.global_workspace_root}/.cache
 global_tmp: ${.global_workspace_root}/.tmp
 # project specific paths
 project_root: ${oc.select:..project_root,${alt:${oc.env:HYFI_PROJECT_ROOT,null},${get_original_cwd:}}}
-project_data_root: ${oc.select:..project_data_root,${alt:${oc.env:HYFI_PROJECT_DATA_ROOT,null},${.project_root}/workspace}}
-project_archive: ${.project_data_root}/archive
-project_datasets: ${.project_data_root}/datasets
-project_models: ${.project_data_root}/models
-project_modules: ${.project_data_root}/modules
-project_outputs: ${.project_data_root}/outputs
-project_logs: ${.project_data_root}/logs
-project_library: ${.project_data_root}/libs
-project_cache: ${.project_data_root}/.cache
-project_tmp: ${.project_data_root}/.tmp
+project_workspace_name: ${oc.select:..project_workspace_name,${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}}
+project_workspace_root: ${.project_root}/${.project_workspace_name}
+project_archive: ${.project_workspace_root}/archive
+project_datasets: ${.project_workspace_root}/datasets
+project_models: ${.project_workspace_root}/models
+project_modules: ${.project_workspace_root}/modules
+project_outputs: ${.project_workspace_root}/outputs
+project_logs: ${.project_workspace_root}/logs
+project_library: ${.project_workspace_root}/libs
+project_cache: ${.project_workspace_root}/.cache
+project_tmp: ${.project_workspace_root}/.tmp
```

### Comparing `entelecheia-0.2.2/src/entelecheia/conf/project/__init__.yaml` & `entelecheia-0.2.3/src/entelecheia/conf/project/__init__.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
-task_name: ${alt:${oc.env:HYFI_TASK_NAME,null},default-task}
+task_name: ${oc.select:..task_name,${alt:${oc.env:HYFI_TASK_NAME,null},default-task}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
-project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${get_original_cwd:}}
-project_data_root: ${alt:${oc.env:HYFI_PROJECT_DATA_ROOT,null},${.project_root}/workspace}
-global_workspace_root: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_ROOT,null},${__home_path__:}/.hyfi}
-global_data_root: ${alt:${oc.env:HYFI_GLOBAL_DATA_ROOT,null},${.global_workspace_root}/data}
+project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
+project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
+global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
+global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
+num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
 use_wandb: false
-verbose: false
+verbose: ${alt:${oc.env:HYFI_VERBOSE,null},false}
```

### Comparing `entelecheia-0.2.2/PKG-INFO` & `entelecheia-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.2.2
+Version: 0.2.3
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.5.1,<0.6.0)
+Requires-Dist: hyfi (>=0.12.2,<0.13.0)
 Project-URL: Repository, https://github.com/entelecheia/entelecheia
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 
 [![home-img]][home-url]
 [![course-img]][course-url]
```

