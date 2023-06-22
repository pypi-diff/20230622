# Comparing `tmp/patch-cli-0.2.7.tar.gz` & `tmp/patch-cli-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patch-cli-0.2.7.tar", last modified: Fri May 19 21:00:16 2023, max compression
+gzip compressed data, was "patch-cli-0.2.8.tar", last modified: Thu Jun 22 16:27:49 2023, max compression
```

## Comparing `patch-cli-0.2.7.tar` & `patch-cli-0.2.8.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.141518 patch-cli-0.2.7/
--rw-r--r--   0 gunner     (501) staff       (20)      655 2023-01-12 18:07:47.000000 patch-cli-0.2.7/.pat-complete.fish
--rw-r--r--   0 gunner     (501) staff       (20)      654 2023-01-12 18:07:47.000000 patch-cli-0.2.7/.pat-complete.sh
--rw-r--r--   0 gunner     (501) staff       (20)      946 2023-01-12 18:07:47.000000 patch-cli-0.2.7/.pat-complete.zsh
--rw-r--r--   0 gunner     (501) staff       (20)     9304 2023-01-12 18:07:47.000000 patch-cli-0.2.7/LICENSE.md
--rw-r--r--   0 gunner     (501) staff       (20)      159 2023-02-13 19:38:49.000000 patch-cli-0.2.7/MANIFEST.in
--rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-05-19 21:00:16.141641 patch-cli-0.2.7/PKG-INFO
--rw-r--r--   0 gunner     (501) staff       (20)     2653 2023-02-27 17:45:34.000000 patch-cli-0.2.7/README.md
--rw-r--r--   0 gunner     (501) staff       (20)        6 2023-05-19 20:51:31.000000 patch-cli-0.2.7/VERSION
--rw-r--r--   0 gunner     (501) staff       (20)       19 2023-01-12 18:07:47.000000 patch-cli-0.2.7/pat.bat
--rw-r--r--   0 gunner     (501) staff       (20)      963 2023-01-12 18:07:47.000000 patch-cli-0.2.7/pat.py
--rw-r--r--   0 gunner     (501) staff       (20)       91 2023-02-13 19:37:47.000000 patch-cli-0.2.7/pyproject.toml
--rw-r--r--   0 gunner     (501) staff       (20)     1580 2023-05-19 21:00:16.142021 patch-cli-0.2.7/setup.cfg
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.120121 patch-cli-0.2.7/src/
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.123279 patch-cli-0.2.7/src/patch/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/__init__.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.124101 patch-cli-0.2.7/src/patch/auth/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/auth/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     5088 2023-04-06 22:23:48.000000 patch-cli-0.2.7/src/patch/auth/auth_client.py
--rw-r--r--   0 gunner     (501) staff       (20)     2852 2023-03-22 14:46:09.000000 patch-cli-0.2.7/src/patch/auth/auth_forms.py
--rw-r--r--   0 gunner     (501) staff       (20)     1856 2023-05-05 21:30:32.000000 patch-cli-0.2.7/src/patch/auth/auth_token.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.125414 patch-cli-0.2.7/src/patch/cli/
--rw-r--r--   0 gunner     (501) staff       (20)     1684 2023-04-19 14:52:13.000000 patch-cli-0.2.7/src/patch/cli/__init__.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.127620 patch-cli-0.2.7/src/patch/cli/commands/
--rw-r--r--   0 gunner     (501) staff       (20)     2262 2023-01-17 11:15:41.000000 patch-cli-0.2.7/src/patch/cli/commands/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     4476 2023-02-27 17:45:34.000000 patch-cli-0.2.7/src/patch/cli/commands/access.py
--rw-r--r--   0 gunner     (501) staff       (20)     8684 2023-03-22 14:46:09.000000 patch-cli-0.2.7/src/patch/cli/commands/admin.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.128294 patch-cli-0.2.7/src/patch/cli/commands/alpha/
--rw-r--r--   0 gunner     (501) staff       (20)      231 2023-04-19 14:52:13.000000 patch-cli-0.2.7/src/patch/cli/commands/alpha/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      299 2023-04-19 14:52:13.000000 patch-cli-0.2.7/src/patch/cli/commands/alpha/package.py
--rw-r--r--   0 gunner     (501) staff       (20)     2821 2023-03-22 14:46:09.000000 patch-cli-0.2.7/src/patch/cli/commands/connector.py
--rw-r--r--   0 gunner     (501) staff       (20)    28241 2023-05-19 20:53:02.000000 patch-cli-0.2.7/src/patch/cli/commands/dataset.py
--rw-r--r--   0 gunner     (501) staff       (20)     3477 2023-05-01 15:38:50.000000 patch-cli-0.2.7/src/patch/cli/commands/destination.py
--rw-r--r--   0 gunner     (501) staff       (20)     3058 2023-04-12 15:20:59.000000 patch-cli-0.2.7/src/patch/cli/commands/login.py
--rw-r--r--   0 gunner     (501) staff       (20)      511 2023-04-12 15:20:57.000000 patch-cli-0.2.7/src/patch/cli/commands/logout.py
--rw-r--r--   0 gunner     (501) staff       (20)     1800 2023-03-22 14:46:09.000000 patch-cli-0.2.7/src/patch/cli/commands/playground.py
--rw-r--r--   0 gunner     (501) staff       (20)     5808 2023-05-01 15:38:50.000000 patch-cli-0.2.7/src/patch/cli/commands/source.py
--rw-r--r--   0 gunner     (501) staff       (20)      886 2023-01-17 11:15:41.000000 patch-cli-0.2.7/src/patch/cli/commands/token.py
--rw-r--r--   0 gunner     (501) staff       (20)     1901 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/commands/user.py
--rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/eap.py
--rw-r--r--   0 gunner     (501) staff       (20)     1244 2023-01-17 11:15:41.000000 patch-cli-0.2.7/src/patch/cli/patch_click_context.py
--rw-r--r--   0 gunner     (501) staff       (20)      446 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/phone_number_param_type.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.128684 patch-cli-0.2.7/src/patch/cli/remote/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/remote/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      676 2023-05-08 21:20:59.000000 patch-cli-0.2.7/src/patch/cli/remote/dataset_client.py
--rw-r--r--   0 gunner     (501) staff       (20)      542 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/remote/source_client.py
--rw-r--r--   0 gunner     (501) staff       (20)     2122 2023-03-01 17:45:31.000000 patch-cli-0.2.7/src/patch/cli/styled.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.130268 patch-cli-0.2.7/src/patch/cli/tools/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      368 2023-03-22 14:46:09.000000 patch-cli-0.2.7/src/patch/cli/tools/base64_encryption.py
--rw-r--r--   0 gunner     (501) staff       (20)     4483 2023-05-01 15:38:50.000000 patch-cli-0.2.7/src/patch/cli/tools/config.py
--rw-r--r--   0 gunner     (501) staff       (20)     1314 2023-04-19 20:57:35.000000 patch-cli-0.2.7/src/patch/cli/tools/config_interactive.py
--rw-r--r--   0 gunner     (501) staff       (20)     1055 2023-05-01 15:38:50.000000 patch-cli-0.2.7/src/patch/cli/tools/config_non_interactive.py
--rw-r--r--   0 gunner     (501) staff       (20)     1207 2023-04-19 16:48:56.000000 patch-cli-0.2.7/src/patch/cli/tools/config_spec.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.130603 patch-cli-0.2.7/src/patch/cli/tools/connectors/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/connectors/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     5960 2023-04-28 21:47:49.000000 patch-cli-0.2.7/src/patch/cli/tools/connectors/connector_spec.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.131658 patch-cli-0.2.7/src/patch/cli/tools/datasets/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/datasets/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     1011 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/datasets/curl_renderer.py
--rw-r--r--   0 gunner     (501) staff       (20)     1639 2023-05-11 16:01:56.000000 patch-cli-0.2.7/src/patch/cli/tools/datasets/diff_renderer.py
--rw-r--r--   0 gunner     (501) staff       (20)     5674 2023-05-13 14:28:55.000000 patch-cli-0.2.7/src/patch/cli/tools/datasets/endpoint_renderer.py
--rw-r--r--   0 gunner     (501) staff       (20)     2069 2023-03-01 16:12:11.000000 patch-cli-0.2.7/src/patch/cli/tools/datasets/row_table_renderer.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.131941 patch-cli-0.2.7/src/patch/cli/tools/destinations/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-04-19 21:08:16.000000 patch-cli-0.2.7/src/patch/cli/tools/destinations/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     3336 2023-05-01 15:38:50.000000 patch-cli-0.2.7/src/patch/cli/tools/destinations/destination_spec.py
--rw-r--r--   0 gunner     (501) staff       (20)      730 2023-05-18 01:55:49.000000 patch-cli-0.2.7/src/patch/cli/tools/field_spec.py
--rw-r--r--   0 gunner     (501) staff       (20)      352 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/filters_reader.py
--rw-r--r--   0 gunner     (501) staff       (20)      456 2023-01-13 17:10:04.000000 patch-cli-0.2.7/src/patch/cli/tools/json_reader.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.132557 patch-cli-0.2.7/src/patch/cli/tools/state/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-04-12 15:20:57.000000 patch-cli-0.2.7/src/patch/cli/tools/state/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      299 2023-04-12 15:20:59.000000 patch-cli-0.2.7/src/patch/cli/tools/state/auth_state_transfer.py
--rw-r--r--   0 gunner     (501) staff       (20)     1257 2023-04-12 15:20:57.000000 patch-cli-0.2.7/src/patch/cli/tools/state/bi_directional_state_transfer.py
--rw-r--r--   0 gunner     (501) staff       (20)      612 2023-04-12 15:20:57.000000 patch-cli-0.2.7/src/patch/cli/tools/state/state_transfer.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.133871 patch-cli-0.2.7/src/patch/cli/tools/tables/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/__init__.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.136103 patch-cli-0.2.7/src/patch/cli/tools/tables/components/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     1064 2023-01-18 15:21:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/container_panel.py
--rw-r--r--   0 gunner     (501) staff       (20)     2693 2023-02-27 17:45:34.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/hierarchy_renderer.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.136367 patch-cli-0.2.7/src/patch/cli/tools/tables/components/list_tools/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/list_tools/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     1643 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/list_tools/data_list.py
--rw-r--r--   0 gunner     (501) staff       (20)     2093 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_quota.py
--rw-r--r--   0 gunner     (501) staff       (20)      309 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_search.py
--rw-r--r--   0 gunner     (501) staff       (20)     1458 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_summary.py
--rw-r--r--   0 gunner     (501) staff       (20)     3897 2023-05-13 14:28:48.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular.py
--rw-r--r--   0 gunner     (501) staff       (20)      470 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_all_in.py
--rw-r--r--   0 gunner     (501) staff       (20)      904 2023-05-01 20:19:18.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_appendable.py
--rw-r--r--   0 gunner     (501) staff       (20)      949 2023-05-01 20:19:04.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_positional.py
--rw-r--r--   0 gunner     (501) staff       (20)     1699 2023-01-30 13:11:07.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py
--rw-r--r--   0 gunner     (501) staff       (20)     1602 2023-05-10 19:24:01.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.136831 patch-cli-0.2.7/src/patch/cli/tools/tables/components/viewport/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/viewport/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     4760 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/viewport/cursor_controller.py
--rw-r--r--   0 gunner     (501) staff       (20)     3321 2023-01-19 15:51:24.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/components/viewport/viewport.py
--rw-r--r--   0 gunner     (501) staff       (20)      478 2023-03-22 14:46:09.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/renders.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.138175 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      962 2023-05-03 15:09:16.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/columns_row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)      431 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/panel_tabular_row.py
--rw-r--r--   0 gunner     (501) staff       (20)      583 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)     1258 2023-05-10 19:16:05.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_data_row.py
--rw-r--r--   0 gunner     (501) staff       (20)     1149 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)      266 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_row_collection_quota_aware.py
--rw-r--r--   0 gunner     (501) staff       (20)     1371 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)      423 2023-03-01 17:45:31.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/source_app.css
--rw-r--r--   0 gunner     (501) staff       (20)     4490 2023-05-10 19:28:53.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/source_app.py
--rw-r--r--   0 gunner     (501) staff       (20)      382 2023-05-10 19:52:32.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/source_data.py
--rw-r--r--   0 gunner     (501) staff       (20)     7738 2023-05-19 18:39:17.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/source_metadata_client.py
--rw-r--r--   0 gunner     (501) staff       (20)     5646 2023-05-05 21:30:32.000000 patch-cli-0.2.7/src/patch/cli/tools/tables/state_manager.py
--rw-r--r--   0 gunner     (501) staff       (20)      187 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/debug.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.138617 patch-cli-0.2.7/src/patch/gql/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/gql/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     3024 2023-04-06 22:23:04.000000 patch-cli-0.2.7/src/patch/gql/client.py
--rw-r--r--   0 gunner     (501) staff       (20)    15317 2023-05-19 20:48:32.000000 patch-cli-0.2.7/src/patch/gql/schema.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.139949 patch-cli-0.2.7/src/patch/storage/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/storage/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      391 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/storage/auth.py
--rw-r--r--   0 gunner     (501) staff       (20)      163 2023-04-06 22:16:46.000000 patch-cli-0.2.7/src/patch/storage/domain.py
--rw-r--r--   0 gunner     (501) staff       (20)      148 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/storage/generic_payload.py
--rw-r--r--   0 gunner     (501) staff       (20)      955 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/storage/generic_storage_file.py
--rw-r--r--   0 gunner     (501) staff       (20)      398 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/storage/state_file.py
--rw-r--r--   0 gunner     (501) staff       (20)     1472 2023-04-06 14:53:28.000000 patch-cli-0.2.7/src/patch/storage/storage.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.140242 patch-cli-0.2.7/src/patch/tp/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/tp/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.7/src/patch/tp/phone_number.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-05-19 21:00:16.141377 patch-cli-0.2.7/src/patch_cli.egg-info/
--rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-05-19 21:00:16.000000 patch-cli-0.2.7/src/patch_cli.egg-info/PKG-INFO
--rw-r--r--   0 gunner     (501) staff       (20)     4376 2023-05-19 21:00:16.000000 patch-cli-0.2.7/src/patch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 gunner     (501) staff       (20)        1 2023-05-19 21:00:16.000000 patch-cli-0.2.7/src/patch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 gunner     (501) staff       (20)       44 2023-05-19 21:00:16.000000 patch-cli-0.2.7/src/patch_cli.egg-info/entry_points.txt
--rw-r--r--   0 gunner     (501) staff       (20)      236 2023-05-19 21:00:16.000000 patch-cli-0.2.7/src/patch_cli.egg-info/requires.txt
--rw-r--r--   0 gunner     (501) staff       (20)        6 2023-05-19 21:00:16.000000 patch-cli-0.2.7/src/patch_cli.egg-info/top_level.txt
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.748335 patch-cli-0.2.8/
+-rw-r--r--   0 gunner     (501) staff       (20)      655 2023-06-22 15:42:14.000000 patch-cli-0.2.8/.pat-complete.fish
+-rw-r--r--   0 gunner     (501) staff       (20)      654 2023-06-22 15:42:10.000000 patch-cli-0.2.8/.pat-complete.sh
+-rw-r--r--   0 gunner     (501) staff       (20)      946 2023-06-22 15:42:06.000000 patch-cli-0.2.8/.pat-complete.zsh
+-rw-r--r--   0 gunner     (501) staff       (20)     9304 2023-01-12 18:07:47.000000 patch-cli-0.2.8/LICENSE.md
+-rw-r--r--   0 gunner     (501) staff       (20)      159 2023-02-13 19:38:49.000000 patch-cli-0.2.8/MANIFEST.in
+-rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-06-22 16:27:49.748433 patch-cli-0.2.8/PKG-INFO
+-rw-r--r--   0 gunner     (501) staff       (20)     2653 2023-02-27 17:45:34.000000 patch-cli-0.2.8/README.md
+-rw-r--r--   0 gunner     (501) staff       (20)        6 2023-06-22 16:27:28.000000 patch-cli-0.2.8/VERSION
+-rw-r--r--   0 gunner     (501) staff       (20)       19 2023-01-12 18:07:47.000000 patch-cli-0.2.8/pat.bat
+-rw-r--r--   0 gunner     (501) staff       (20)      963 2023-01-12 18:07:47.000000 patch-cli-0.2.8/pat.py
+-rw-r--r--   0 gunner     (501) staff       (20)       91 2023-02-13 19:37:47.000000 patch-cli-0.2.8/pyproject.toml
+-rw-r--r--   0 gunner     (501) staff       (20)     1580 2023-06-22 16:27:49.748778 patch-cli-0.2.8/setup.cfg
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.730724 patch-cli-0.2.8/src/
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.733796 patch-cli-0.2.8/src/patch/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/__init__.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.734237 patch-cli-0.2.8/src/patch/auth/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/auth/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5088 2023-04-06 22:23:48.000000 patch-cli-0.2.8/src/patch/auth/auth_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2852 2023-03-22 14:46:09.000000 patch-cli-0.2.8/src/patch/auth/auth_forms.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1856 2023-05-05 21:30:32.000000 patch-cli-0.2.8/src/patch/auth/auth_token.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.734858 patch-cli-0.2.8/src/patch/cli/
+-rw-r--r--   0 gunner     (501) staff       (20)     1684 2023-04-19 14:52:13.000000 patch-cli-0.2.8/src/patch/cli/__init__.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.736956 patch-cli-0.2.8/src/patch/cli/commands/
+-rw-r--r--   0 gunner     (501) staff       (20)     2262 2023-01-17 11:15:41.000000 patch-cli-0.2.8/src/patch/cli/commands/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4476 2023-02-27 17:45:34.000000 patch-cli-0.2.8/src/patch/cli/commands/access.py
+-rw-r--r--   0 gunner     (501) staff       (20)     8684 2023-03-22 14:46:09.000000 patch-cli-0.2.8/src/patch/cli/commands/admin.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.737245 patch-cli-0.2.8/src/patch/cli/commands/alpha/
+-rw-r--r--   0 gunner     (501) staff       (20)      231 2023-04-19 14:52:13.000000 patch-cli-0.2.8/src/patch/cli/commands/alpha/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      299 2023-04-19 14:52:13.000000 patch-cli-0.2.8/src/patch/cli/commands/alpha/package.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2821 2023-03-22 14:46:09.000000 patch-cli-0.2.8/src/patch/cli/commands/connector.py
+-rw-r--r--   0 gunner     (501) staff       (20)    29678 2023-06-22 15:47:14.000000 patch-cli-0.2.8/src/patch/cli/commands/dataset.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3477 2023-05-01 15:38:50.000000 patch-cli-0.2.8/src/patch/cli/commands/destination.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3058 2023-04-12 15:20:59.000000 patch-cli-0.2.8/src/patch/cli/commands/login.py
+-rw-r--r--   0 gunner     (501) staff       (20)      511 2023-04-12 15:20:57.000000 patch-cli-0.2.8/src/patch/cli/commands/logout.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1800 2023-03-22 14:46:09.000000 patch-cli-0.2.8/src/patch/cli/commands/playground.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5808 2023-05-01 15:38:50.000000 patch-cli-0.2.8/src/patch/cli/commands/source.py
+-rw-r--r--   0 gunner     (501) staff       (20)      886 2023-01-17 11:15:41.000000 patch-cli-0.2.8/src/patch/cli/commands/token.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1901 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/commands/user.py
+-rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/eap.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1244 2023-01-17 11:15:41.000000 patch-cli-0.2.8/src/patch/cli/patch_click_context.py
+-rw-r--r--   0 gunner     (501) staff       (20)      446 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/phone_number_param_type.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.737638 patch-cli-0.2.8/src/patch/cli/remote/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/remote/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      705 2023-05-26 16:36:48.000000 patch-cli-0.2.8/src/patch/cli/remote/dataset_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)      542 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/remote/source_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2122 2023-03-01 17:45:31.000000 patch-cli-0.2.8/src/patch/cli/styled.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.738855 patch-cli-0.2.8/src/patch/cli/tools/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      368 2023-03-22 14:46:09.000000 patch-cli-0.2.8/src/patch/cli/tools/base64_encryption.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4483 2023-05-01 15:38:50.000000 patch-cli-0.2.8/src/patch/cli/tools/config.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1314 2023-04-19 20:57:35.000000 patch-cli-0.2.8/src/patch/cli/tools/config_interactive.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1055 2023-05-01 15:38:50.000000 patch-cli-0.2.8/src/patch/cli/tools/config_non_interactive.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1207 2023-04-19 16:48:56.000000 patch-cli-0.2.8/src/patch/cli/tools/config_spec.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.739065 patch-cli-0.2.8/src/patch/cli/tools/connectors/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/connectors/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5960 2023-04-28 21:47:49.000000 patch-cli-0.2.8/src/patch/cli/tools/connectors/connector_spec.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.739667 patch-cli-0.2.8/src/patch/cli/tools/datasets/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/datasets/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1011 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/datasets/curl_renderer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1673 2023-05-22 15:14:02.000000 patch-cli-0.2.8/src/patch/cli/tools/datasets/diff_renderer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5674 2023-05-13 14:28:55.000000 patch-cli-0.2.8/src/patch/cli/tools/datasets/endpoint_renderer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2069 2023-03-01 16:12:11.000000 patch-cli-0.2.8/src/patch/cli/tools/datasets/row_table_renderer.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.739963 patch-cli-0.2.8/src/patch/cli/tools/destinations/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-04-19 21:08:16.000000 patch-cli-0.2.8/src/patch/cli/tools/destinations/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3336 2023-05-01 15:38:50.000000 patch-cli-0.2.8/src/patch/cli/tools/destinations/destination_spec.py
+-rw-r--r--   0 gunner     (501) staff       (20)      730 2023-05-18 01:55:49.000000 patch-cli-0.2.8/src/patch/cli/tools/field_spec.py
+-rw-r--r--   0 gunner     (501) staff       (20)      352 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/filters_reader.py
+-rw-r--r--   0 gunner     (501) staff       (20)      456 2023-01-13 17:10:04.000000 patch-cli-0.2.8/src/patch/cli/tools/json_reader.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.740671 patch-cli-0.2.8/src/patch/cli/tools/state/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-04-12 15:20:57.000000 patch-cli-0.2.8/src/patch/cli/tools/state/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      299 2023-04-12 15:20:59.000000 patch-cli-0.2.8/src/patch/cli/tools/state/auth_state_transfer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1257 2023-04-12 15:20:57.000000 patch-cli-0.2.8/src/patch/cli/tools/state/bi_directional_state_transfer.py
+-rw-r--r--   0 gunner     (501) staff       (20)      612 2023-04-12 15:20:57.000000 patch-cli-0.2.8/src/patch/cli/tools/state/state_transfer.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.741690 patch-cli-0.2.8/src/patch/cli/tools/tables/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/__init__.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.743590 patch-cli-0.2.8/src/patch/cli/tools/tables/components/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1064 2023-01-18 15:21:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/container_panel.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2693 2023-02-27 17:45:34.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/hierarchy_renderer.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.743833 patch-cli-0.2.8/src/patch/cli/tools/tables/components/list_tools/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/list_tools/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1643 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/list_tools/data_list.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2093 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_quota.py
+-rw-r--r--   0 gunner     (501) staff       (20)      309 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_search.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1458 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_summary.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3897 2023-05-13 14:28:48.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular.py
+-rw-r--r--   0 gunner     (501) staff       (20)      470 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_all_in.py
+-rw-r--r--   0 gunner     (501) staff       (20)      904 2023-05-01 20:19:18.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_appendable.py
+-rw-r--r--   0 gunner     (501) staff       (20)      949 2023-05-01 20:19:04.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_positional.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1699 2023-01-30 13:11:07.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1602 2023-05-10 19:24:01.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.744241 patch-cli-0.2.8/src/patch/cli/tools/tables/components/viewport/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/viewport/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4760 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/viewport/cursor_controller.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3321 2023-01-19 15:51:24.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/components/viewport/viewport.py
+-rw-r--r--   0 gunner     (501) staff       (20)      478 2023-03-22 14:46:09.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/renders.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.745348 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      962 2023-05-03 15:09:16.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/columns_row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)      431 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/panel_tabular_row.py
+-rw-r--r--   0 gunner     (501) staff       (20)      583 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1258 2023-05-10 19:16:05.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_data_row.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1149 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)      266 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_row_collection_quota_aware.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1371 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)      423 2023-03-01 17:45:31.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/source_app.css
+-rw-r--r--   0 gunner     (501) staff       (20)     4490 2023-05-10 19:28:53.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/source_app.py
+-rw-r--r--   0 gunner     (501) staff       (20)      382 2023-05-10 19:52:32.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/source_data.py
+-rw-r--r--   0 gunner     (501) staff       (20)     7785 2023-05-22 21:43:25.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/source_metadata_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5646 2023-05-05 21:30:32.000000 patch-cli-0.2.8/src/patch/cli/tools/tables/state_manager.py
+-rw-r--r--   0 gunner     (501) staff       (20)      187 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/debug.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.745705 patch-cli-0.2.8/src/patch/gql/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/gql/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3024 2023-04-06 22:23:04.000000 patch-cli-0.2.8/src/patch/gql/client.py
+-rw-r--r--   0 gunner     (501) staff       (20)    15549 2023-05-30 19:28:21.000000 patch-cli-0.2.8/src/patch/gql/schema.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.746883 patch-cli-0.2.8/src/patch/storage/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/storage/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      391 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/storage/auth.py
+-rw-r--r--   0 gunner     (501) staff       (20)      163 2023-04-06 22:16:46.000000 patch-cli-0.2.8/src/patch/storage/domain.py
+-rw-r--r--   0 gunner     (501) staff       (20)      148 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/storage/generic_payload.py
+-rw-r--r--   0 gunner     (501) staff       (20)      955 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/storage/generic_storage_file.py
+-rw-r--r--   0 gunner     (501) staff       (20)      398 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/storage/state_file.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1472 2023-04-06 14:53:28.000000 patch-cli-0.2.8/src/patch/storage/storage.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.747278 patch-cli-0.2.8/src/patch/tp/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/tp/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.8/src/patch/tp/phone_number.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-06-22 16:27:49.748196 patch-cli-0.2.8/src/patch_cli.egg-info/
+-rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-06-22 16:27:49.000000 patch-cli-0.2.8/src/patch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 gunner     (501) staff       (20)     4376 2023-06-22 16:27:49.000000 patch-cli-0.2.8/src/patch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 gunner     (501) staff       (20)        1 2023-06-22 16:27:49.000000 patch-cli-0.2.8/src/patch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 gunner     (501) staff       (20)       44 2023-06-22 16:27:49.000000 patch-cli-0.2.8/src/patch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 gunner     (501) staff       (20)      236 2023-06-22 16:27:49.000000 patch-cli-0.2.8/src/patch_cli.egg-info/requires.txt
+-rw-r--r--   0 gunner     (501) staff       (20)        6 2023-06-22 16:27:49.000000 patch-cli-0.2.8/src/patch_cli.egg-info/top_level.txt
```

### Comparing `patch-cli-0.2.7/.pat-complete.fish` & `patch-cli-0.2.8/.pat-complete.fish`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/.pat-complete.sh` & `patch-cli-0.2.8/.pat-complete.sh`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/.pat-complete.zsh` & `patch-cli-0.2.8/.pat-complete.zsh`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/LICENSE.md` & `patch-cli-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/PKG-INFO` & `patch-cli-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-cli
-Version: 0.2.7
+Version: 0.2.8
 Summary: Spin up analytics APIs over your data in minutes, without writing any code.
 Home-page: https://www.patch.tech/
 Download-URL: https://docs.patch.tech/command-line-interface/installation
 Author: Patch Enterprises
 Author-email: eng@patch.tech
 Project-URL: Changelog, https://patch.releases.live/
 Project-URL: Documentation, https://docs.patch.tech/command-line-interface/basic-usage
```

### Comparing `patch-cli-0.2.7/README.md` & `patch-cli-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/pat.py` & `patch-cli-0.2.8/pat.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/setup.cfg` & `patch-cli-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/auth/auth_client.py` & `patch-cli-0.2.8/src/patch/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/auth/auth_forms.py` & `patch-cli-0.2.8/src/patch/auth/auth_forms.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/auth/auth_token.py` & `patch-cli-0.2.8/src/patch/auth/auth_token.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/__init__.py` & `patch-cli-0.2.8/src/patch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/__init__.py` & `patch-cli-0.2.8/src/patch/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/access.py` & `patch-cli-0.2.8/src/patch/cli/commands/access.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/admin.py` & `patch-cli-0.2.8/src/patch/cli/commands/admin.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/connector.py` & `patch-cli-0.2.8/src/patch/cli/commands/connector.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/dataset.py` & `patch-cli-0.2.8/src/patch/cli/commands/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,20 @@
         'datasetName': name,
         'tables': config["tables"],
     }
     if "destinations" in config:
         config_vals["destinations"] = config["destinations"]
     return config_vals
 
-def update_dataset_interactive(console, name, interface, meta):
+def update_dataset_interactive(console, version, name, interface, meta):
 
     source_app = SourceApp(meta=meta)
     source_app.run()
     if meta.source_data.is_ready:
-        return interface.build_update_dataset_input(dataset_name=name, tables=meta.source_data.selected_tables)
+        return interface.build_update_dataset_input(dataset_name=name, version=version, tables=meta.source_data.selected_tables)
 
     return None
 
 
 @dataset.command(cls=StyledCommand, help='Configure dataset')
 @click.option('-c', '--config', type=click.File(mode='r'), help='Configuration file')
 @click.argument('name', type=click.STRING)
@@ -155,18 +155,19 @@
     segments = [name]
     if size is not None:
         segments.append(f"({size})")
     return " ".join(segments)
 
 @dataset.command(cls=StyledCommand, help='Update a configured dataset')
 @click.option('-t', '--edit-tables', help="Update a configured dataset's tables", is_flag=True)
+@click.option('-y', '--assume-yes', '--yes', help='Skip confirmation', is_flag=True)
 @click.argument('name', type=click.STRING)
 @with_as_tenant()
 @pass_obj()
-def update(patch_ctx: PatchClickContext, edit_tables, name):
+def update(patch_ctx: PatchClickContext, edit_tables, name, assume_yes):
     console = patch_ctx.console
     with active_source(patch_ctx) as local_state:
         client = patch_ctx.gql_client
         source_id = local_state.active_source_id
         dataset_client = DatasetClient(console, client, source_id=source_id)
         dataset = dataset_client.query_dataset(name)
         if not dataset:
@@ -176,26 +177,26 @@
         meta = SourceMeta(source_data=interface.get_source_metadata(dataset))
         selected_tables = list(filter(lambda i: i not in meta.source_data.obsolete_tables, meta.source_data.selected_tables))
 
         if not (meta.source_data.tables or selected_tables):
             console.print(f"No tables found in active source [blue]{local_state.active_source_name}[/blue].")
             return None
         if edit_tables:
-            update_dataset_input = update_dataset_interactive(console, name, interface, meta)
+            update_dataset_input = update_dataset_interactive(console, dataset['latestVersion'], name, interface, meta)
         else:
-            update_dataset_input = interface.build_update_dataset_input(dataset_name=name,
-                                                                    tables=meta.source_data.selected_tables)
+            update_dataset_input = interface.build_update_dataset_input(dataset_name=name, version=dataset['latestVersion'],
+                                                                        tables=meta.source_data.selected_tables)
         
-        if update_dataset_input:
-            diff = generate_diff(console, local_state.active_source_name,
+        if update_dataset_input and not assume_yes:
+            diff = generate_diff(console, local_state.active_source_name, dataset['latestVersion'],
                                     dataset.tables, list(filter(lambda i: i not in meta.source_data.obsolete_tables, meta.source_data.selected_tables)))
         else:
             diff = False
 
-        if diff:
+        if diff or assume_yes:
             update = mutate_update_dataset(client, console, update_dataset_input)
             if update.ok:
                 console.print("[bold green]Dataset update submitted![/bold green] "
                         f"Your dataset will now be updated to version {update.createdVersion}.")
             else:
                 console.print("[bold_red]Error: There was an error processing your update. Consider trying again, or reach out to your Patch contact.[/bold_red]")
         else:
@@ -221,34 +222,55 @@
             console.print("[yellow]No datasets found[/yellow]")
         else:
             has_edges = any(t.edges for d in dataset_list for t in d.tables)
 
             table = Table(title="Datasets", box=box.ROUNDED, border_style="grey37")
             table.add_column("Name", style="cyan", no_wrap=True, overflow="fold")
             table.add_column("ID", style="yellow", overflow="fold")
-            table.add_column("Tables", justify="left", overflow="fold")
             if has_edges:
                 table.add_column("Edges", justify="left", overflow="fold")
 
             dataset_list_sorted = sorted(dataset_list, key=lambda d: d.name)
             for dataset_elem in dataset_list_sorted:
-                table_names = []
-                for t in dataset_elem.tables:
-                    table_info = [t.lastRowCount, t.tableState]
-                    if t.lastCdcSuccessTimeAgo:
-                        table_info.append("Synced " + t.lastCdcSuccessTimeAgo + " ago")
-                    table_names.append(render_table(t.name, table_info))
-                joined_table_names = join_with_limit(table_names).replace("[", "").replace("]", "").replace("'", "")
                 if has_edges:
                     edge_descriptions = create_edge_descriptions(dataset_elem.tables, console)
-                    table.add_row(dataset_elem.name, dataset_elem.id, joined_table_names, edge_descriptions)
+                    table.add_row(dataset_elem.name, dataset_elem.id, edge_descriptions)
                 else:
-                    table.add_row(dataset_elem.name, dataset_elem.id, joined_table_names)
+                    table.add_row(dataset_elem.name, dataset_elem.id)
             console.print(table)
 
+@dataset.command(cls=StyledCommand, help='List a dataset\'s table information across versions')
+@click.argument('name', type=click.STRING)
+@with_as_tenant()
+@pass_obj()
+def describe(patch_ctx: PatchClickContext, name: str):
+    console = patch_ctx.console
+    with active_source(patch_ctx, show_state=True) as local_state:
+        client = patch_ctx.gql_client
+        dataset_client = DatasetClient(console, client, source_id=local_state.active_source_id)
+        dataset = dataset_client.query_dataset(name)
+
+        if not dataset:
+            raise Exception(f"Dataset {name} does not exist.")
+
+        table = Table(title=f"{name} Table Information", box=box.ROUNDED, border_style="grey37")
+        table.add_column("Dataset Version", style="cyan", no_wrap=True, overflow="fold")
+        table.add_column("Table Name", style="yellow", overflow="fold")
+        table.add_column("Rows", justify="left", overflow="fold")
+        table.add_column("State", justify="left", overflow="fold")
+        table.add_column("Last Sync", justify="left", overflow="fold")
+
+        version_list_sorted = sorted(dataset.versions, key=lambda d: d.version, reverse=True)
+        for dataset_version in version_list_sorted:
+            for i, t in enumerate(sorted(dataset_version.tables, key=lambda t: t.name)):
+                table_state = f"[red]{t.tableState}[/red]" if t.tableState == "ERROR" else f"[green]{t.tableState}[/green]"
+                last_sync = (t.lastCdcSuccessTimeAgo + " ago") if t.lastCdcSuccessTimeAgo else "[red]Unsynced[/red]"
+                end_section = i == len(dataset_version.tables) - 1
+                table.add_row(str(dataset_version.version), t.name, str(t.lastRowCount), table_state, last_sync, end_section=end_section)
+        console.print(table)
 
 @dataset.command(cls=StyledCommand, help='Remove dataset')
 @click.argument('name', type=click.STRING)
 @click.option('-y', '--assume-yes', '--yes', help='Skip confirmation', is_flag=True)
 @with_as_tenant()
 @pass_obj()
 def remove(patch_ctx: PatchClickContext, name, assume_yes):
```

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/destination.py` & `patch-cli-0.2.8/src/patch/cli/commands/destination.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/login.py` & `patch-cli-0.2.8/src/patch/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/playground.py` & `patch-cli-0.2.8/src/patch/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/source.py` & `patch-cli-0.2.8/src/patch/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/token.py` & `patch-cli-0.2.8/src/patch/cli/commands/token.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/commands/user.py` & `patch-cli-0.2.8/src/patch/cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/patch_click_context.py` & `patch-cli-0.2.8/src/patch/cli/patch_click_context.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/remote/dataset_client.py` & `patch-cli-0.2.8/src/patch/cli/remote/dataset_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 
     def query_dataset(self, name):
         gql_query = self.gql_client.prepare_query('datasetByName', input={
             'sourceId': self.source_id,
             'datasetName': name
         })
         with gql_query as q:
-            q.__fields__('id', 'tables')
+            q.__fields__('id', 'tables', 'versions', 'latestVersion')
         with self.console.status("[bold green]Checking dataset name...[/bold green]") as _status:
             return gql_query.execute()
```

### Comparing `patch-cli-0.2.7/src/patch/cli/remote/source_client.py` & `patch-cli-0.2.8/src/patch/cli/remote/source_client.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/styled.py` & `patch-cli-0.2.8/src/patch/cli/styled.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/config.py` & `patch-cli-0.2.8/src/patch/cli/tools/config.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/config_interactive.py` & `patch-cli-0.2.8/src/patch/cli/tools/config_interactive.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/config_non_interactive.py` & `patch-cli-0.2.8/src/patch/cli/tools/config_non_interactive.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/config_spec.py` & `patch-cli-0.2.8/src/patch/cli/tools/config_spec.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/connectors/connector_spec.py` & `patch-cli-0.2.8/src/patch/cli/tools/connectors/connector_spec.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/datasets/curl_renderer.py` & `patch-cli-0.2.8/src/patch/cli/tools/datasets/curl_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/datasets/diff_renderer.py` & `patch-cli-0.2.8/src/patch/cli/tools/datasets/diff_renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def format_tables(source, console, tables_before, tables_after): # source should become a table field eventually, and version should be recieved from a dataset query
     formatted_tables_before = {table.name: {"source": source , "columns": [{column.name: column.graphqlType.upper()} for column in table.columns]} for table in tables_before}
     formatted_tables_after = {table.name: {"source": source , "columns": [{column.name: column.type} for column in table.columns if column.color != "bright_red"]} for table in tables_after}
     json1_obj = json.dumps(formatted_tables_before, sort_keys=True, indent=2).splitlines()
     json2_obj = json.dumps(formatted_tables_after, sort_keys=True, indent=2).splitlines()
     return json1_obj, json2_obj
 
-def generate_diff(console, source, dataset_before, dataset_after):
+def generate_diff(console, source, version, dataset_before, dataset_after):
     json1_obj, json2_obj = format_tables(source, console, dataset_before, dataset_after)
 
     if json1_obj == json2_obj:
         console.print("[red]Error: pat dataset update was run, but no differences in the schema were detected.[/red]")
         return None
 
     diff_generator = difflib.ndiff(json1_obj, json2_obj)
@@ -21,10 +21,10 @@
     for line in diff_generator:
         if line.startswith('+'):
             console.print(f"[green]{line}[/green]")  # Green for additions
         elif line.startswith('-'):
             console.print(f"[red]{line}[/red]")  # Red for deletions
         else:
             console.print(f"[white]{line}[/white]")
-    confirmation = Confirm.ask(f"Approve the following changes?",
+    confirmation = Confirm.ask(f"Update dataset to version [blue]{(version + 1)}[/blue]?",
                                console=console)
     return confirmation
```

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/datasets/endpoint_renderer.py` & `patch-cli-0.2.8/src/patch/cli/tools/datasets/endpoint_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/datasets/row_table_renderer.py` & `patch-cli-0.2.8/src/patch/cli/tools/datasets/row_table_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/destinations/destination_spec.py` & `patch-cli-0.2.8/src/patch/cli/tools/destinations/destination_spec.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/field_spec.py` & `patch-cli-0.2.8/src/patch/cli/tools/field_spec.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/state/bi_directional_state_transfer.py` & `patch-cli-0.2.8/src/patch/cli/tools/state/bi_directional_state_transfer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/state/state_transfer.py` & `patch-cli-0.2.8/src/patch/cli/tools/state/state_transfer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/container_panel.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/container_panel.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/hierarchy_renderer.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/hierarchy_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/list_tools/data_list.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/list_tools/data_list.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_quota.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_quota.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_summary.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_summary.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_appendable.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_appendable.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_positional.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_positional.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/viewport/cursor_controller.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/viewport/cursor_controller.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/components/viewport/viewport.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/components/viewport/viewport.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/rows/columns_row_collection.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/rows/columns_row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/rows/row_collection.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/rows/row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_data_row.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_data_row.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_row_collection.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/source_app.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/source_app.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/source_metadata_client.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/source_metadata_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,24 +143,25 @@
             })
         return {
             'sourceId': self.source_id,
             'datasetName': dataset_name,
             'tables': tables_input
         }
     
-    def build_update_dataset_input(self, dataset_name, tables):
+    def build_update_dataset_input(self, version, dataset_name, tables):
         tables_input = []
         for table in tables:
             columns_input = []
             for column in table.columns:
                 if column.selected is True:
                     columns_input.append({'columnName': column.name})
             tables_input.append({
                 'tableId': table.id,
                 'ingestMode': default_ingest_mode,
                 'primaryKey': columns_input
             })
         return {
             'sourceId': self.source_id,
             'datasetName': dataset_name,
-            'tables': tables_input
+            'tables': tables_input,
+            'version': (version + 1)
         }
```

### Comparing `patch-cli-0.2.7/src/patch/cli/tools/tables/state_manager.py` & `patch-cli-0.2.8/src/patch/cli/tools/tables/state_manager.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/gql/client.py` & `patch-cli-0.2.8/src/patch/gql/client.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/gql/schema.py` & `patch-cli-0.2.8/src/patch/gql/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,20 +181,25 @@
     destination = non_null(Destination)
 
 
 class DatasetDestinationInput(Input):
     name = non_null(str)
     mapping = list_of(non_null(TableMappingInput))
 
+class DatasetVersion(Type):
+    version = non_null(int)
+    tables = non_null(list_of(non_null(DatasetTable)))
 
 class Dataset(Type):
     id = non_null(str)
     name = non_null(str)
+    versions = non_null(list_of(non_null(DatasetVersion)))
     tables = non_null(list_of(non_null('DatasetTable')))
     destinations = non_null(list_of(non_null(DatasetDestination)))
+    latestVersion = non_null(int)
 
 
 class QueryAuth(Type):
     accessToken = non_null(str)
 
 
 class DataAccessKey(Type):
@@ -261,14 +266,15 @@
     tables = non_null(list_of(non_null(CreateDatasetTableInput)))
     destinations = list_of(non_null(DatasetDestinationInput))
 
 class UpdateDatasetInput(Input):
     sourceId = non_null(str)
     datasetName = non_null(str)
     tables = non_null(list_of(non_null(UpdateDatasetTableInput)))
+    version = non_null(int)
 
 class DestinationInput(Input):
     name = non_null(str)
     type = non_null(DestinationType)
     batchApi = BatchApiDestinationInput
```

### Comparing `patch-cli-0.2.7/src/patch/storage/generic_storage_file.py` & `patch-cli-0.2.8/src/patch/storage/generic_storage_file.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch/storage/storage.py` & `patch-cli-0.2.8/src/patch/storage/storage.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.7/src/patch_cli.egg-info/PKG-INFO` & `patch-cli-0.2.8/src/patch_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-cli
-Version: 0.2.7
+Version: 0.2.8
 Summary: Spin up analytics APIs over your data in minutes, without writing any code.
 Home-page: https://www.patch.tech/
 Download-URL: https://docs.patch.tech/command-line-interface/installation
 Author: Patch Enterprises
 Author-email: eng@patch.tech
 Project-URL: Changelog, https://patch.releases.live/
 Project-URL: Documentation, https://docs.patch.tech/command-line-interface/basic-usage
```

### Comparing `patch-cli-0.2.7/src/patch_cli.egg-info/SOURCES.txt` & `patch-cli-0.2.8/src/patch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

