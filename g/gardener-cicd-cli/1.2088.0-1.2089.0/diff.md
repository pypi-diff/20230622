# Comparing `tmp/gardener-cicd-cli-1.2088.0.tar.gz` & `tmp/gardener-cicd-cli-1.2089.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2088.0.tar", last modified: Tue Jun 20 08:00:13 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2089.0.tar", last modified: Thu Jun 22 06:35:33 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2088.0.tar` & `gardener-cicd-cli-1.2089.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:13.773014 gardener-cicd-cli-1.2088.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-20 08:00:13.769014 gardener-cicd-cli-1.2088.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:13.765014 gardener-cicd-cli-1.2088.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:13.769014 gardener-cicd-cli-1.2088.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     8114 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11329 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     7669 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12219 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/productutil_v2.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/whdutil.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:13.769014 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-20 08:00:13.000000 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-20 08:00:13.000000 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 08:00:13.000000 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-20 08:00:13.000000 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-20 08:00:13.000000 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 08:00:13.000000 gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 08:00:13.773014 gardener-cicd-cli-1.2088.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-06-20 07:59:01.000000 gardener-cicd-cli-1.2088.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:35:33.559577 gardener-cicd-cli-1.2089.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-22 06:35:33.559577 gardener-cicd-cli-1.2089.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:35:33.555577 gardener-cicd-cli-1.2089.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:35:33.559577 gardener-cicd-cli-1.2089.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     8114 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/productutil_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/whdutil.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:35:33.559577 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-22 06:35:33.000000 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-22 06:35:33.000000 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 06:35:33.000000 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-22 06:35:33.000000 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-22 06:35:33.000000 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 06:35:33.000000 gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 06:35:33.559577 gardener-cicd-cli-1.2089.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-06-22 06:25:16.000000 gardener-cicd-cli-1.2089.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2088.0/bin/component-cli` & `gardener-cicd-cli-1.2089.0/bin/component-cli`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2089.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/bin/purge_history` & `gardener-cicd-cli-1.2089.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/compliance.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,26 +45,28 @@
     left_name: str
     right_name: str
     left_version: str
     right_version: str
     ctx_repo_url: str
     exclude_component_names: list[str] = None
     exclude_component_resource_names: list[ComponentResourceNames] = None
+    resource_types: list[str] = None
     name_template: str = None
     name_template_expr: str = None
     outfile_prefix: str = 'resource-diff'
 
 
 def diff(
     left_name: str=None,
     right_name: str=None,
     left_version: str=None,
     right_version: str=None,
     name_template: str=None,
     name_template_expr: str=None,
+    resource_types: [str]=None,
     ctx_repo_url: str=None,
     cache_dir: str=_cfg.ctx.cache_dir,
     defaults_file: str=None,
     outfile_prefix: str='resource-diff'
 ):
     if defaults_file:
         params = ci.util.parse_yaml_file(defaults_file)
@@ -81,14 +83,16 @@
         params['right_version'] = right_version
     if ctx_repo_url:
         params['ctx_repo_url'] = ctx_repo_url
     if name_template:
         params['name_template'] = name_template
     if name_template_expr:
         params['name_template_expr'] = name_template
+    if resource_types:
+        params['resource_types'] = resource_types
 
     try:
         parsed = dacite.from_dict(
             data_class=DiffArguments,
             data=params,
         )
     except:
@@ -147,14 +151,23 @@
     def resource_version_id(component, resource):
         # ignore component-version, honour resource-version
         return component.name, resource.name, resource.version
 
     def iter_resources_with_ids(components):
         for c in components:
             for r in c.resources:
+                if parsed.resource_types:
+                    if isinstance(r.type, cm.ResourceType):
+                        resource_type = r.type.value
+                    else:
+                        resource_type = r.type
+
+                    if not resource_type in parsed.resource_types:
+                        continue
+
                 if parsed.exclude_component_resource_names:
                     skip = True
                     for component_resource_name in parsed.exclude_component_resource_names:
                         if re.fullmatch(component_resource_name.component_name, c.name) \
                             and \
                             re.fullmatch(component_resource_name.resource_name, r.name):
                             break
```

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_ci/whdutil.py` & `gardener-cicd-cli-1.2089.0/gardener_ci/whdutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2089.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2088.0/setup.py` & `gardener-cicd-cli-1.2089.0/setup.py`

 * *Files identical despite different names*

