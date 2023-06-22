# Comparing `tmp/dagworks-sdk-0.0.10.tar.gz` & `tmp/dagworks-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks-sdk-0.0.10.tar", last modified: Thu Jun 22 18:39:45 2023, max compression
+gzip compressed data, was "dagworks-sdk-0.0.9.tar", last modified: Wed Jun 21 04:37:32 2023, max compression
```

## Comparing `dagworks-sdk-0.0.10.tar` & `dagworks-sdk-0.0.9.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.135736 dagworks-sdk-0.0.10/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2212 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/LICENSE
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4696 2023-06-22 18:39:45.135564 dagworks-sdk-0.0.10/PKG-INFO
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3655 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/README.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/pyproject.toml
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       14 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/requirements-test.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      213 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/requirements.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2023-06-22 18:39:45.135787 dagworks-sdk-0.0.10/setup.cfg
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      115 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/setup.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.108076 dagworks-sdk-0.0.10/src/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.109265 dagworks-sdk-0.0.10/src/dagworks/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1093 2023-06-22 18:38:45.000000 dagworks-sdk-0.0.10/src/dagworks/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.110053 dagworks-sdk-0.0.10/src/dagworks/api/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.110952 dagworks-sdk-0.0.10/src/dagworks/api/api_client/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      152 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.111098 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.112136 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3379 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2926 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5383 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4111 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4813 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.114141 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3035 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5855 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4711 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5053 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4516 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4994 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8029 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5693 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5511 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5779 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6327 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.115149 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4421 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5087 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6058 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6286 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5367 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2817 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/client.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      470 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/errors.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.123861 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4237 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2443 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/api_key_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1982 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/dependency.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2706 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1285 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3019 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1268 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2766 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2480 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_function.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3778 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_node.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1692 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1175 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_node_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/organization_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/paged_api_key_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2238 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/paged_project_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/paged_run_log_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1649 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/phone_home_result.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1977 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1179 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_in_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4499 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1165 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_out_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3909 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_in_git.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_in_git_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1243 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_in_git_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5339 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1203 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_version_info.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5848 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_with_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1244 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1282 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1422 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/python_type.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1791 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_data.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5416 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1185 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1171 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_run_log.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6517 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1163 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7054 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3710 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/task_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1198 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/task_run_result_summary.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      226 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/task_run_status.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3189 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2916 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1586 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/user_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4362 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/visibility_full.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3802 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/visibility_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2306 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/who_am_i_result.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      993 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/api_client/types.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9831 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/clients.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1161 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/constants.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1311 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.124341 dagworks-sdk-0.0.10/src/dagworks/cli/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2025 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/cli.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6513 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.124503 dagworks-sdk-0.0.10/src/dagworks/cli/templates/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.125242 dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      123 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      307 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       51 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2698 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      697 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.125408 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.126026 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      351 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      520 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2528 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.126207 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       26 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.126861 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      232 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      480 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      309 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      678 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.127014 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.127319 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1577 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.127683 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      157 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      149 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      674 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.127836 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.128861 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      488 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3736 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      598 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2531 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1402 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      477 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.129085 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.130021 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1447 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      369 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      710 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      931 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      744 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.130161 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)   991302 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      679 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    14619 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/driver.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.132004 dagworks-sdk-0.0.10/src/dagworks/parsing/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/parsing/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2394 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/parsing/dagtypes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7810 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/parsing/parse.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.132296 dagworks-sdk-0.0.10/src/dagworks/telemetry/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7465 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.133889 dagworks-sdk-0.0.10/src/dagworks/tracking/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3486 2023-06-22 18:14:39.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/dataframe_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5969 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6307 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/pandas_col_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5691 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/pandas_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7107 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/polars_col_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5549 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/polars_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9073 2023-06-22 18:38:45.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/runs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2827 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2411 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/src/dagworks/tracking/trackingtypes.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.134622 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4696 2023-06-22 18:39:45.000000 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8764 2023-06-22 18:39:45.000000 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2023-06-22 18:39:45.000000 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       50 2023-06-22 18:39:45.000000 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      192 2023-06-22 18:39:45.000000 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        9 2023-06-22 18:39:45.000000 dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:39:45.135217 dagworks-sdk-0.0.10/tests/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2970 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/tests/test_driver.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3343 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.10/tests/test_telemetry.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6185 2023-06-22 18:38:45.000000 dagworks-sdk-0.0.10/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.688913 dagworks-sdk-0.0.9/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/LICENSE
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-06-21 04:37:32.688514 dagworks-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       14 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      213 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-06-21 04:37:32.689013 dagworks-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.627471 dagworks-sdk-0.0.9/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.630709 dagworks-sdk-0.0.9/src/dagworks/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-06-21 04:37:19.000000 dagworks-sdk-0.0.9/src/dagworks/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.632750 dagworks-sdk-0.0.9/src/dagworks/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.634548 dagworks-sdk-0.0.9/src/dagworks/api/api_client/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.634891 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.637068 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3379 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2926 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5383 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4111 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4813 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.641261 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3035 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5855 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4711 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5053 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4516 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4994 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8029 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5693 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5511 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5779 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6327 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.643477 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4421 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5087 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6058 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6286 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5367 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2817 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/client.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      470 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/errors.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.662016 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4237 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/dependency.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2706 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1285 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3019 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1268 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_function.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_node.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_node_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/organization_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/paged_api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/paged_project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/paged_run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/phone_home_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4499 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_in_git.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_in_git_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_in_git_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5339 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5848 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_with_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/python_type.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_data.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5416 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1185 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_run_log.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6517 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7054 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/task_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/task_run_result_summary.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/task_run_status.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3189 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2916 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/user_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/visibility_full.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3802 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/visibility_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/who_am_i_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      993 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/api_client/types.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9831 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1161 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.663174 dagworks-sdk-0.0.9/src/dagworks/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2025 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6513 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.663622 dagworks-sdk-0.0.9/src/dagworks/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.665351 dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.665718 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.667589 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.667972 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.669505 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.670032 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.670748 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.671416 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.671743 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.673768 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.674107 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.676232 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.676568 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    14619 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.680569 dagworks-sdk-0.0.9/src/dagworks/parsing/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/parsing/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/parsing/dagtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/parsing/parse.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.681525 dagworks-sdk-0.0.9/src/dagworks/telemetry/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.685106 dagworks-sdk-0.0.9/src/dagworks/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3486 2023-06-21 04:37:19.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/dataframe_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6307 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/pandas_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5691 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/pandas_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7107 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/polars_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5549 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/polars_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8991 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2827 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/src/dagworks/tracking/trackingtypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.686907 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-06-21 04:37:32.000000 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8764 2023-06-21 04:37:32.000000 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-06-21 04:37:32.000000 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-06-21 04:37:32.000000 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      192 2023-06-21 04:37:32.000000 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-06-21 04:37:32.000000 dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:37:32.687947 dagworks-sdk-0.0.9/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/tests/test_telemetry.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6103 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.9/tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.10/LICENSE` & `dagworks-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/PKG-INFO` & `dagworks-sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.10
+Version: 0.0.9
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.10/README.md` & `dagworks-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/pyproject.toml` & `dagworks-sdk-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/api/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 0, 10)
+DAGWORKS_API_URL = "https://api.app.dagworks.io"
+DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/client.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/client.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/api_key_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/dependency.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/dependency.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_in.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_dag.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_function.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_function.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_node.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_node.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_node_dependencies.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_node_dependencies.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/hamilton_node_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/hamilton_node_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/organization_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/organization_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/paged_api_key_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/paged_api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/paged_project_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/paged_project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/paged_run_log_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/paged_run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/phone_home_result.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/phone_home_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_in.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_in_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_out_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_in_git.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_in_git.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_in_git_dag.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_in_git_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_in_git_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_in_git_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_version_info.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_with_dag.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_with_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/python_type.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/python_type.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_data.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_data.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_config.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_inputs.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_run_log.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_run_log.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_in_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_config.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_inputs.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run_config.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/task_run.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/task_run_result_summary.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/task_run_result_summary.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/user_out.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/user_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/visibility_full.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/visibility_full.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/visibility_in.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/visibility_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/models/who_am_i_result.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/models/who_am_i_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/api_client/types.py` & `dagworks-sdk-0.0.9/src/dagworks/api/api_client/types.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/clients.py` & `dagworks-sdk-0.0.9/src/dagworks/api/clients.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/constants.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,10 +13,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-DAGWORKS_API_URL = "https://api.app.dagworks.io"
-DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks-sdk-0.0.10/src/dagworks/api/projecttypes.py` & `dagworks-sdk-0.0.9/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/cli.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/initialize.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/common/run.sh.jinja2` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/iris_loader.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks-sdk-0.0.9/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/driver.py` & `dagworks-sdk-0.0.9/src/dagworks/driver.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/parsing/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/parsing/dagtypes.py` & `dagworks-sdk-0.0.9/src/dagworks/parsing/dagtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/parsing/parse.py` & `dagworks-sdk-0.0.9/src/dagworks/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/telemetry/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/telemetry/telemetry.py` & `dagworks-sdk-0.0.9/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/__init__.py` & `dagworks-sdk-0.0.9/src/dagworks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+__version__ = (0, 0, 9)
```

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/dataframe_stats.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/dataframe_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/example_tracking.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/pandas_col_stats.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/pandas_col_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/pandas_stats.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/pandas_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/polars_col_stats.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/polars_col_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/polars_stats.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/polars_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/runs.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/runs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import functools
 import logging
 import sys
 import time as py_time
 import traceback
 from contextlib import contextmanager
-from datetime import datetime, timezone
+from datetime import datetime
 from typing import Any, Callable, Dict, List
 
 from hamilton import base
 from hamilton import node as h_node
 from hamilton.data_quality import base as dq_base
 
 from dagworks.tracking.trackingtypes import DAGRun, Status, TaskRun
@@ -91,20 +91,20 @@
         self.task_map: Dict[str, TaskRun] = {}
         self.update_status(Status.UNINITIALIZED)
 
     def clock_start(self):
         """Called at start of run"""
         logger.info("Clocked beginning of run")
         self.status = Status.RUNNING
-        self.start_time = datetime.now(timezone.utc)
+        self.start_time = datetime.now()
 
     def clock_end(self, status: Status):
         """Called at end of run"""
         logger.info(f"Clocked end of run with status: {status}")
-        self.end_time = datetime.now(timezone.utc)
+        self.end_time = datetime.now()
         self.status = status
 
     def update_task(self, task_name: str, task_run: TaskRun):
         """Updates a task"""
         self.task_map.update({task_name: task_run})
         logger.debug(f"Updating task: {task_name} with data: {task_run}")
 
@@ -187,36 +187,36 @@
         logger.debug(f"Executing node: {node.name}")
         # If the hamilton_tracking state hasn't started
         if self.tracking_state.status == Status.UNINITIALIZED:
             self.tracking_state.update_status(Status.RUNNING)
 
         task_run = TaskRun(node_name=node.name)  # node run.
         task_run.status = Status.RUNNING
-        task_run.start_time = datetime.now(timezone.utc)
+        task_run.start_time = datetime.now()
         self.tracking_state.update_task(node.name, task_run)
         try:
             result = original_execute_node(node, kwargs)
             task_run.status = Status.SUCCESS
             task_run.result_type = type(result)
             task_run.result_summary = process_result(result, node)  # add node
-            task_run.end_time = datetime.now(timezone.utc)
+            task_run.end_time = datetime.now()
             self.tracking_state.update_task(node.name, task_run)
             logger.debug(f"Node: {node.name} ran successfully")
             return result
         except dq_base.DataValidationError as e:
             task_run.status = Status.FAILURE
-            task_run.end_time = datetime.now(timezone.utc)
+            task_run.end_time = datetime.now()
             task_run.error = serialize_data_quality_error(e)
             self.tracking_state.update_status(Status.FAILURE)
             self.tracking_state.update_task(node.name, task_run)
             logger.debug(f"Node: {node.name} encountered data quality issue...")
             raise e
         except Exception as e:
             task_run.status = Status.FAILURE
-            task_run.end_time = datetime.now(timezone.utc)
+            task_run.end_time = datetime.now()
             task_run.error = serialize_error()
             self.tracking_state.update_status(Status.FAILURE)
             self.tracking_state.update_task(node.name, task_run)
             logger.debug(f"Node: {node.name} failed to run...")
             raise e
```

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/stats.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks/tracking/trackingtypes.py` & `dagworks-sdk-0.0.9/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.10
+Version: 0.0.9
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.10/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks-sdk-0.0.9/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/tests/test_driver.py` & `dagworks-sdk-0.0.9/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/tests/test_telemetry.py` & `dagworks-sdk-0.0.9/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.10/tests/test_tracking.py` & `dagworks-sdk-0.0.9/tests/test_tracking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-from datetime import datetime, timezone
+from datetime import datetime
 from typing import Any, Callable, Dict, List
 
 import pytest
 from hamilton import base
 
 import tests.resources.basic_dag_with_config
 from dagworks import driver
@@ -49,16 +49,16 @@
             name=name,
             version_info=version_info,
             version_info_schema=0,
             version_info_type="git",
             dag_pointer="s3://path/to/dag",
             dag_schema_version=0,
             logged_by=0,
-            created_at=datetime.now(timezone.utc),
-            updated_at=datetime.now(timezone.utc),
+            created_at=datetime.now(),
+            updated_at=datetime.now(),
             id=0,
             slug="slug",
         )
 
     @track_calls
     def validate_auth(self):
         pass
@@ -67,16 +67,16 @@
     def ensure_project_exists(self, project_id: int) -> ProjectOut:
         tags = ProjectOutTags()
         tags.additional_properties = {}
         return ProjectOut(
             name="",
             description="",
             tags=ProjectOutTags(),
-            created_at=datetime.now(timezone.utc),
-            updated_at=datetime.now(timezone.utc),
+            created_at=datetime.now(),
+            updated_at=datetime.now(),
             owner="elijah",
             permissions=VisibilityFull([], [], [], []),
             documentation=[],
             can_write=True,
         )
 
     @track_calls
@@ -96,19 +96,19 @@
     state = TrackingState("test")
     state.clock_start()
     state.update_task(
         task_name="foo",
         task_run=TaskRun(
             node_name="node_1",
             status=Status.RUNNING,
-            start_time=datetime.now(timezone.utc),
+            start_time=datetime.now(),
         ),
     )
     task = state.task_map["foo"]
-    task.end_time = datetime.now(timezone.utc)
+    task.end_time = datetime.now()
     task.status = Status.SUCCESS
     state.update_task(task_name="foo", task_run=task)
     state.clock_end(Status.SUCCESS)
     run = state.get()
     assert len(run.tasks) == 1
     assert run.status == Status.SUCCESS
     assert run.run_id == "test"
```

