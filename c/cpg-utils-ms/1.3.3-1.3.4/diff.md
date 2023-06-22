# Comparing `tmp/cpg-utils-ms-1.3.3.tar.gz` & `tmp/cpg-utils-ms-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-ms-1.3.3.tar", last modified: Thu Jan 26 17:25:56 2023, max compression
+gzip compressed data, was "cpg-utils-ms-1.3.4.tar", last modified: Thu Jun 22 21:21:55 2023, max compression
```

## Comparing `cpg-utils-ms-1.3.3.tar` & `cpg-utils-ms-1.3.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:25:56.551334 cpg-utils-ms-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-01-26 17:25:56.551334 cpg-utils-ms-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:25:56.551334 cpg-utils-ms-1.3.3/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/deploy_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    16616 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/cpg_utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:25:56.551334 cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-01-26 17:25:56.000000 cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-26 17:25:56.000000 cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 17:25:56.000000 cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-26 17:25:56.000000 cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-26 17:25:56.000000 cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 17:25:56.551334 cpg-utils-ms-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:25:56.551334 cpg-utils-ms-1.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/test_cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-26 17:24:30.000000 cpg-utils-ms-1.3.3/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.842728 cpg-utils-ms-1.3.4/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/deploy_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_storage.py
```

### Comparing `cpg-utils-ms-1.3.3/LICENSE` & `cpg-utils-ms-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/PKG-INFO` & `cpg-utils-ms-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils-ms
-Version: 1.3.3
+Version: 1.3.4
 Summary: Library of convenience functions specific to the CPG (MS version)
 Home-page: https://github.com/gregsmi/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-ms-1.3.3/README.md` & `cpg-utils-ms-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/__init__.py` & `cpg-utils-ms-1.3.4/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/auth.py` & `cpg-utils-ms-1.3.4/cpg_utils/auth.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/cloud.py` & `cpg-utils-ms-1.3.4/cpg_utils/cloud.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 """Convenience functions related to cloud infrastructure."""
 
 import json
 import os
+import re
 import traceback
 
 from google.auth import (
     credentials as google_auth_credentials,
     environment_vars,
     exceptions,
 )
 from google.auth import jwt
 from google.auth._default import (
     _AUTHORIZED_USER_TYPE,
-    _HELP_MESSAGE,
     _SERVICE_ACCOUNT_TYPE,
     _VALID_TYPES,
 )
+
+# pylint: disable=no-name-in-module
 from google.cloud import secretmanager
 from google.oauth2 import credentials as oauth2_credentials, service_account
 import google.api_core.exceptions
 import google.auth.transport
 from google.auth.transport import requests
 import google.oauth2
+from cloudpathlib import AnyPath
+
+from cpg_utils.config import get_config
+
+_CLOUD_SDK_MISSING_CREDENTIALS = """\
+Your default credentials were not found. To set up Application Default Credentials, \
+see https://cloud.google.com/docs/authentication/external/set-up-adc for more information.\
+"""
 
 
 def email_from_id_token(id_token_jwt: str) -> str:
     """Decodes the ID token (JWT) to get the email address of the caller.
 
     See http://bit.ly/2YAIkzy for details.
 
@@ -279,8 +289,61 @@
     )
 
     for checker in checkers:
         current_credentials = checker()
         if current_credentials is not None:
             return current_credentials
 
-    raise exceptions.DefaultCredentialsError(_HELP_MESSAGE)
+    raise exceptions.DefaultCredentialsError(_CLOUD_SDK_MISSING_CREDENTIALS)
+
+
+def get_cached_group_members(
+    group, members_cache_location: str | None = None
+) -> set[str]:
+    """
+    Get cached members of a group, based on the members_cache_location
+    """
+    group_name = group.split('@')[0]
+
+    if not members_cache_location:
+        config = get_config()
+        members_cache_location = config['infrastructure']['members_cache_location']
+
+    pathname = os.path.join(members_cache_location, group_name + '-members.txt')  # type: ignore
+
+    with AnyPath(pathname).open() as f:
+        return set(line.strip() for line in f.readlines() if line.strip())
+
+
+def is_member_in_cached_group(
+    group, member, members_cache_location: str | None = None
+) -> bool:
+    """
+    Check if a member is in a group, based on the infrastructure config
+    """
+    return member.lower() in get_cached_group_members(
+        group, members_cache_location=members_cache_location
+    )
+
+
+def get_path_components_from_gcp_path(path: str) -> dict[str, str]:
+    """
+    Return the {bucket_name}, {dataset}, {bucket_type}, {subdir}, and {file} for GS only paths
+    Uses regex to match the full bucket name, dataset name, bucket type (e.g. 'test', 'main-upload', 'release'),
+    subdirectory, and the file name.
+    """
+
+    bucket_types = ['archive', 'hail', 'main', 'test', 'release']
+
+    # compile pattern matching all CPG bucket formats
+    gspath_pattern = re.compile(
+        r'gs://(?P<bucket>cpg-(?P<dataset>[\w-]+)-(?P<bucket_type>['
+        + '|'.join(s for s in bucket_types)
+        + r']+[-\w]*))/(?P<suffix>.+/)?(?P<file>.*)$'
+    )
+
+    # if a match succeeds, return the key: value dictionary
+    if path_match := gspath_pattern.match(path):
+        return path_match.groupdict()
+
+    # raise an error if the input String was not a valid CPG bucket path
+    raise ValueError('The input String did not match a valid GCP path')
```

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-ms-1.3.4/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/config.py` & `cpg-utils-ms-1.3.4/cpg_utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """
     if _env_var := os.environ.get('CPG_CONFIG_PATH'):
         config_paths = _env_var.split(',') + config_paths
 
     set_config_paths(config_paths)
 
 
-def get_config() -> frozendict:
+def get_config(print_config=True) -> frozendict:
     """Returns the configuration dictionary.
 
     Call `set_config_paths` beforehand to override the default path.
     See `read_configs` for the path value semantics.
 
     Notes
     -----
@@ -104,17 +104,18 @@
         assert (
             _config_paths
         ), 'Either set the CPG_CONFIG_PATH environment variable or call set_config_paths'
 
         _config = read_configs(_config_paths)
 
         # Print the config content, which is helpful for debugging.
-        print(
-            f'Configuration at {",".join(_config_paths)}:\n{toml.dumps(dict(_config))}'
-        )
+        if print_config:
+            print(
+                f'Configuration at {",".join(_config_paths)}:\n{toml.dumps(dict(_config))}'
+            )
 
         # Update deployment config if available.
         if 'CPG_DEPLOY_CONFIG' in _config:
             set_deploy_config(DeployConfig(**_config['CPG_DEPLOY_CONFIG']))
 
 
     return _config
```

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/creds.py` & `cpg-utils-ms-1.3.4/cpg_utils/creds.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/deploy_config.py` & `cpg-utils-ms-1.3.4/cpg_utils/deploy_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/git.py` & `cpg-utils-ms-1.3.4/cpg_utils/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     try:
         return subprocess.check_output(command).decode().strip()
     # Handle and rethrow KeyboardInterrupt error to stop global exception catch
     # pylint: disable=try-except-raise
     except KeyboardInterrupt:
         raise
     except subprocess.CalledProcessError as e:
-        raise Exception(
+        raise RuntimeError(
             f"Couldn't call {description} by calling '{' '.join(command)}', {e}"
         ) from e
     except Exception as e:
-        raise Exception(
+        raise RuntimeError(
             f"Couldn't process {description} through calling '{' '.join(command)}', {e}"
         ) from e
 
 
 def get_git_root_relative_path_from_absolute(full_path: str) -> str:
     """
     Convert an absolute path within a git repo to a path relative to the git root.
@@ -180,18 +180,18 @@
                 organisation = match.group('org')
 
         elif remote_name.startswith('git@'):
             match = re.match(r'git@[A-z0-9.]+?:(?P<org>.+?)/.+$', remote_name)
             if match:
                 organisation = match.group('org')
     except AttributeError as ae:
-        raise Exception(f'Unsupported remote format: "{remote_name}"') from ae
+        raise ValueError(f'Unsupported remote format: "{remote_name}"') from ae
 
     if organisation is None:
-        raise Exception(f'Unsupported remote format: "{remote_name}"')
+        raise ValueError(f'Unsupported remote format: "{remote_name}"')
 
     return organisation
 
 
 def get_repo_name_from_remote(remote_name: str) -> str:
     """
     Get the name of a GitHub repo from a supported organisation
@@ -218,18 +218,18 @@
                 repo = match.group('repo')
 
         elif remote_name.startswith('git@'):
             match = re.match(r'git@[A-z0-9.]+?:.+?/(?P<repo>.+)$', remote_name)
             if match:
                 repo = match.group('repo')
     except AttributeError as ae:
-        raise Exception(f'Unsupported remote format: "{remote_name}"') from ae
+        raise ValueError(f'Unsupported remote format: "{remote_name}"') from ae
 
     if repo is None:
-        raise Exception(f'Unsupported remote format: "{remote_name}"')
+        raise ValueError(f'Unsupported remote format: "{remote_name}"')
 
     if repo.endswith('.git'):
         repo = repo[:-4]
 
     return repo
```

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/hail_batch.py` & `cpg-utils-ms-1.3.4/cpg_utils/hail_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
     `--dataset fewgenomes --access-level test`:
 
     >>> from cpg_utils.hail_batch import dataset_path
     >>> dataset_path('1kg_densified/combined.mt')
     'gs://cpg-fewgenomes-test/1kg_densified/combined.mt'
     >>> dataset_path('1kg_densified/report.html', 'web')
     'gs://cpg-fewgenomes-test-web/1kg_densified/report.html'
+    >>> dataset_path('1kg_densified/report.html', 'web', test=True)
+    'gs://cpg-fewgenomes-test-web/1kg_densified/report.html'
 
     Notes
     -----
     Performs a lookup on the `storage` section of the config file, and the  `workflow/dataset` 
     config variables if not passed in as an  argument. These configuration settings are added 
     automatically by analysis-runner.
 
@@ -166,15 +168,19 @@
 def web_url(suffix: str = '', dataset: str | None = None) -> str:
     """
     Web URL to match the dataset_path of category 'web'.
     """
     return dataset_path(suffix=suffix, dataset=dataset, category='web_url')
 
 
-def output_path(suffix: str, category: Optional[str] = None) -> str:
+def output_path(
+    suffix: str,
+    category: Optional[str] = None,
+    dataset: Optional[str] = None,
+) -> str:
     """
     Returns a full path for the given category and path suffix.
 
     In contrast to the `dataset_path` function, `output_path` takes the
     `workflow/output_prefix` config variable into account.
 
     Examples
@@ -199,21 +205,23 @@
 
     Parameters
     ----------
     suffix : str
         A path suffix to append to the bucket + output directory.
     category : str, optional
         A category like "tmp", "web", etc., defaults to "default" if ommited.
+    dataset : str, optional
+        Dataset name, takes precedence over the `workflow/dataset` config variable
 
     Returns
     -------
     str
     """
     prefix = retrieve(['workflow', 'output_prefix'])
-    return dataset_path(f'{prefix}/{suffix}', category)
+    return dataset_path(f'{prefix}/{suffix}', category, dataset)
 
 
 def image_path(key: str) -> str:
     """
     Returns a path to a container image using key in config's "images" section.
 
     Examples
@@ -287,19 +295,19 @@
     @param b: Hail Batch object.
     @param indices: list of extensions to add to the base fasta file path.
     """
     ref_fasta = get_config()['workflow'].get('ref_fasta') or reference_path(
         'broad/ref_fasta'
     )
     ref_fasta = to_path(ref_fasta)
-    d = dict(
-        base=str(ref_fasta),
-        fai=str(ref_fasta) + '.fai',
-        dict=str(ref_fasta.with_suffix('.dict')),
-    )
+    d = {
+        'base': str(ref_fasta),
+        'fai': str(ref_fasta) + '.fai',
+        'dict': str(ref_fasta.with_suffix('.dict')),
+    }
     if indices:
         for ext in indices:
             d[ext] = f'{ref_fasta}.{ext}'
     return b.read_input_group(**d)
 
 
 def authenticate_cloud_credentials_in_job(
```

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/secrets.py` & `cpg-utils-ms-1.3.4/cpg_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils/storage.py` & `cpg-utils-ms-1.3.4/cpg_utils/storage.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/PKG-INFO` & `cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils-ms
-Version: 1.3.3
+Version: 1.3.4
 Summary: Library of convenience functions specific to the CPG (MS version)
 Home-page: https://github.com/gregsmi/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-ms-1.3.3/cpg_utils_ms.egg-info/SOURCES.txt` & `cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 cpg_utils/cloudpath_hail_az.py
 cpg_utils/config.py
 cpg_utils/creds.py
 cpg_utils/deploy_config.py
 cpg_utils/git.py
 cpg_utils/hail_batch.py
 cpg_utils/secrets.py
+cpg_utils/slack.py
 cpg_utils/storage.py
 cpg_utils_ms.egg-info/PKG-INFO
 cpg_utils_ms.egg-info/SOURCES.txt
 cpg_utils_ms.egg-info/dependency_links.txt
 cpg_utils_ms.egg-info/requires.txt
 cpg_utils_ms.egg-info/top_level.txt
 test/__init__.py
```

### Comparing `cpg-utils-ms-1.3.3/pyproject.toml` & `cpg-utils-ms-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/setup.py` & `cpg-utils-ms-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='cpg-utils-ms',
     # This tag is automatically updated by bumpversion
-    version='1.3.3',
+    version='1.3.4',
     description='Library of convenience functions specific to the CPG (MS version)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/gregsmi/cpg-utils',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `cpg-utils-ms-1.3.3/test/test_auth.py` & `cpg-utils-ms-1.3.4/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/test/test_cloudpath_hail_az.py` & `cpg-utils-ms-1.3.4/test/test_cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/test/test_config.py` & `cpg-utils-ms-1.3.4/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/test/test_secrets.py` & `cpg-utils-ms-1.3.4/test/test_secrets.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.3/test/test_storage.py` & `cpg-utils-ms-1.3.4/test/test_storage.py`

 * *Files identical despite different names*

