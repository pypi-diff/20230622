# Comparing `tmp/chill-0.8.1.tar.gz` & `tmp/chill-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chill-0.8.1.tar", last modified: Sat Jan 23 21:38:14 2021, max compression
+gzip compressed data, was "chill-0.9.0.tar", last modified: Sat Jul  9 21:58:23 2022, max compression
```

## Comparing `chill-0.8.1.tar` & `chill-0.9.0.tar`

### file list

```diff
@@ -1,80 +1,96 @@
-drwxr-xr-x   0 jake      (1000) jake      (1000)        0 2021-01-23 21:38:14.000000 chill-0.8.1/
--rw-r--r--   0 jake      (1000) jake      (1000)     1376 2021-01-23 21:38:14.000000 chill-0.8.1/PKG-INFO
--rw-r--r--   0 jake      (1000) jake      (1000)     3323 2020-06-27 12:20:59.000000 chill-0.8.1/README.md
--rw-r--r--   0 jake      (1000) jake      (1000)       38 2021-01-23 21:38:14.000000 chill-0.8.1/setup.cfg
--rw-r--r--   0 jake      (1000) jake      (1000)     2209 2021-01-23 20:55:52.000000 chill-0.8.1/setup.py
-drwxr-xr-x   0 jake      (1000) jake      (1000)        0 2021-01-23 21:38:14.000000 chill-0.8.1/src/
-drwxr-xr-x   0 jake      (1000) jake      (1000)        0 2021-01-23 21:38:14.000000 chill-0.8.1/src/chill/
--rw-r--r--   0 jake      (1000) jake      (1000)       44 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/__init__.py
--rw-r--r--   0 jake      (1000) jake      (1000)       22 2021-01-23 20:55:52.000000 chill-0.8.1/src/chill/_version.py
--rw-r--r--   0 jake      (1000) jake      (1000)     6764 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/api.py
--rw-r--r--   0 jake      (1000) jake      (1000)    11318 2021-01-21 13:16:05.000000 chill-0.8.1/src/chill/app.py
--rw-r--r--   0 jake      (1000) jake      (1000)       49 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/cache.py
--rw-r--r--   0 jake      (1000) jake      (1000)      351 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/client.py
--rw-r--r--   0 jake      (1000) jake      (1000)     5470 2021-01-21 13:16:05.000000 chill-0.8.1/src/chill/database.py
--rw-r--r--   0 jake      (1000) jake      (1000)     2820 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/migrations.py
--rw-r--r--   0 jake      (1000) jake      (1000)    18913 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/operate.py
--rw-r--r--   0 jake      (1000) jake      (1000)     9824 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/public.py
--rw-r--r--   0 jake      (1000) jake      (1000)     1655 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/pyselect.py
-drwxr-xr-x   0 jake      (1000) jake      (1000)        0 2021-01-23 21:38:14.000000 chill-0.8.1/src/chill/queries/
--rw-r--r--   0 jake      (1000) jake      (1000)       44 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_chill.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      357 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_image.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      280 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      223 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_node_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      134 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_node_picture.sql
--rw-r--r--   0 jake      (1000) jake      (1000)     1022 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_picture.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       83 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_query.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      235 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_route.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      138 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_srcset.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      111 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_staticfile.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       93 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/create_template.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       38 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/delete_node_for_id.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       28 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/drop_chill.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       28 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/drop_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       32 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/drop_node_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       28 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/drop_query.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       28 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/drop_route.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       31 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/drop_template.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      111 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_image.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       55 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       84 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_node_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       91 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_node_picture.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      201 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_picture.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       41 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_query.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       55 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_query_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       96 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_route.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       46 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_staticfile.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       54 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/insert_template.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      254 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_all_chill_nodes.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       20 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_all_nodes.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      172 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_link_node_from_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       78 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_node_from_id.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       82 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_node_from_name.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      143 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_node_from_route.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       50 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_node_node_from_node_id.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       52 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_paths_to_freeze.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       56 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_picture_by_name.sql
--rw-r--r--   0 jake      (1000) jake      (1000)      303 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_picture_for_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       92 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_query_from_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       40 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_query_where_name.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       94 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_route_where_dynamic.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       45 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_staticfile.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       61 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_template.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       98 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/select_template_from_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       40 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/set_current_chill_version.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       74 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/update_node_for_id.sql
--rw-r--r--   0 jake      (1000) jake      (1000)       58 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/queries/update_template_node.sql
--rw-r--r--   0 jake      (1000) jake      (1000)    15538 2021-01-23 21:36:45.000000 chill-0.8.1/src/chill/script.py
--rw-r--r--   0 jake      (1000) jake      (1000)     7538 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/shortcodes.py
--rw-r--r--   0 jake      (1000) jake      (1000)     1693 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/test_api.py
--rw-r--r--   0 jake      (1000) jake      (1000)     2919 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/test_loader.py
--rw-r--r--   0 jake      (1000) jake      (1000)    88467 2021-01-21 13:16:05.000000 chill-0.8.1/src/chill/tests.py
--rw-r--r--   0 jake      (1000) jake      (1000)    11384 2020-06-27 12:20:59.000000 chill-0.8.1/src/chill/yaml_chill_node.py
-drwxr-xr-x   0 jake      (1000) jake      (1000)        0 2021-01-23 21:38:14.000000 chill-0.8.1/src/chill.egg-info/
--rw-r--r--   0 jake      (1000) jake      (1000)     1376 2021-01-23 21:38:13.000000 chill-0.8.1/src/chill.egg-info/PKG-INFO
--rw-r--r--   0 jake      (1000) jake      (1000)     2491 2021-01-23 21:38:14.000000 chill-0.8.1/src/chill.egg-info/SOURCES.txt
--rw-r--r--   0 jake      (1000) jake      (1000)        1 2021-01-23 21:38:13.000000 chill-0.8.1/src/chill.egg-info/dependency_links.txt
--rw-r--r--   0 jake      (1000) jake      (1000)       45 2021-01-23 21:38:13.000000 chill-0.8.1/src/chill.egg-info/entry_points.txt
--rw-r--r--   0 jake      (1000) jake      (1000)        1 2020-06-28 03:57:40.000000 chill-0.8.1/src/chill.egg-info/not-zip-safe
--rw-r--r--   0 jake      (1000) jake      (1000)      131 2021-01-23 21:38:13.000000 chill-0.8.1/src/chill.egg-info/requires.txt
--rw-r--r--   0 jake      (1000) jake      (1000)        6 2021-01-23 21:38:13.000000 chill-0.8.1/src/chill.egg-info/top_level.txt
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.810215 chill-0.9.0/
+-rw-rw-r--   0 jake      (1000) jake      (1000)      188 2022-07-09 21:57:35.000000 chill-0.9.0/.dockerignore
+-rw-rw-r--   0 jake      (1000) jake      (1000)       87 2022-07-09 21:57:35.000000 chill-0.9.0/.flake8
+-rw-rw-r--   0 jake      (1000) jake      (1000)      133 2022-07-09 21:57:35.000000 chill-0.9.0/.gitignore
+-rw-rw-r--   0 jake      (1000) jake      (1000)    35150 2022-07-09 21:57:35.000000 chill-0.9.0/COPYING
+-rw-rw-r--   0 jake      (1000) jake      (1000)     7652 2022-07-09 21:57:35.000000 chill-0.9.0/COPYING.LESSER
+-rw-rw-r--   0 jake      (1000) jake      (1000)     2728 2022-07-09 21:57:35.000000 chill-0.9.0/Dockerfile
+-rw-rw-r--   0 jake      (1000) jake      (1000)       53 2022-07-09 21:57:35.000000 chill-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jake      (1000) jake      (1000)     4645 2022-07-09 21:58:23.810215 chill-0.9.0/PKG-INFO
+-rw-rw-r--   0 jake      (1000) jake      (1000)     3480 2022-07-09 21:57:35.000000 chill-0.9.0/README.md
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.806214 chill-0.9.0/docs/
+-rw-rw-r--   0 jake      (1000) jake      (1000)     2529 2022-07-09 21:57:35.000000 chill-0.9.0/docs/add-page-script.md
+-rw-rw-r--   0 jake      (1000) jake      (1000)     1322 2022-07-09 21:57:35.000000 chill-0.9.0/docs/docker-container-usage.md
+-rw-rw-r--   0 jake      (1000) jake      (1000)     4622 2022-07-09 21:57:35.000000 chill-0.9.0/docs/index.md
+-rw-rw-r--   0 jake      (1000) jake      (1000)      820 2022-07-09 21:57:35.000000 chill-0.9.0/docs/yaml_chill_node_guide_to_dump_and_load.md
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.806214 chill-0.9.0/example/
+-rw-rw-r--   0 jake      (1000) jake      (1000)      573 2022-07-09 21:57:35.000000 chill-0.9.0/example/Dockerfile
+-rw-rw-r--   0 jake      (1000) jake      (1000)      199 2022-07-09 21:57:35.000000 chill-0.9.0/example/chill-data.yaml
+-rw-rw-r--   0 jake      (1000) jake      (1000)     4981 2022-07-09 21:57:35.000000 chill-0.9.0/example/site.cfg
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.806214 chill-0.9.0/example/templates/
+-rw-rw-r--   0 jake      (1000) jake      (1000)      181 2022-07-09 21:57:35.000000 chill-0.9.0/example/templates/homepage.html
+-rw-rw-r--   0 jake      (1000) jake      (1000)      100 2022-07-09 21:57:35.000000 chill-0.9.0/pyproject.toml
+-rw-rw-r--   0 jake      (1000) jake      (1000)      327 2022-07-09 21:57:35.000000 chill-0.9.0/requirements.txt
+-rw-rw-r--   0 jake      (1000) jake      (1000)      118 2022-07-09 21:58:23.810215 chill-0.9.0/setup.cfg
+-rw-rw-r--   0 jake      (1000) jake      (1000)     2002 2022-07-09 21:57:35.000000 chill-0.9.0/setup.py
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.806214 chill-0.9.0/src/
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.810215 chill-0.9.0/src/chill/
+-rw-rw-r--   0 jake      (1000) jake      (1000)       44 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/__init__.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)       22 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/_version.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     8821 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/api.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     9623 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/app.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     6921 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/database.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     3119 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/migrations.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)    11595 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/public.py
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.810215 chill-0.9.0/src/chill/queries/
+-rw-rw-r--   0 jake      (1000) jake      (1000)       44 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_chill.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      357 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_image.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      280 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      223 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_node_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      134 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_node_picture.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)     1022 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_picture.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       83 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_query.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      235 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_route.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      138 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_srcset.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      111 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_staticfile.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       93 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/create_template.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       38 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/delete_node_for_id.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       28 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/drop_chill.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       28 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/drop_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       32 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/drop_node_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       28 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/drop_query.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       28 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/drop_route.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       31 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/drop_template.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      111 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_image.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       55 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       84 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_node_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       91 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_node_picture.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      201 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_picture.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       41 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_query.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       55 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_query_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       96 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_route.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       46 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_staticfile.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       54 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/insert_template.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      254 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_all_chill_nodes.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       20 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_all_nodes.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      172 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_link_node_from_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       78 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_node_from_id.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       82 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_node_from_name.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      143 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_node_from_route.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       50 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_node_node_from_node_id.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       52 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_paths_to_freeze.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       56 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_picture_by_name.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)      303 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_picture_for_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       92 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_query_from_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       40 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_query_where_name.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       94 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_route_where_dynamic.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       45 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_staticfile.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       61 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_template.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       98 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/select_template_from_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       40 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/set_current_chill_version.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       74 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/update_node_for_id.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)       58 2021-10-02 19:08:07.000000 chill-0.9.0/src/chill/queries/update_template_node.sql
+-rw-rw-r--   0 jake      (1000) jake      (1000)    16634 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/script.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     7469 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/shortcodes.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     1709 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/test_api.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)     3221 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/test_loader.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)   108953 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/tests.py
+-rw-rw-r--   0 jake      (1000) jake      (1000)    13031 2022-07-09 21:57:35.000000 chill-0.9.0/src/chill/yaml_chill_node.py
+drwxrwxr-x   0 jake      (1000) jake      (1000)        0 2022-07-09 21:58:23.810215 chill-0.9.0/src/chill.egg-info/
+-rw-rw-r--   0 jake      (1000) jake      (1000)     4645 2022-07-09 21:58:23.000000 chill-0.9.0/src/chill.egg-info/PKG-INFO
+-rw-rw-r--   0 jake      (1000) jake      (1000)     2738 2022-07-09 21:58:23.000000 chill-0.9.0/src/chill.egg-info/SOURCES.txt
+-rw-rw-r--   0 jake      (1000) jake      (1000)        1 2022-07-09 21:58:23.000000 chill-0.9.0/src/chill.egg-info/dependency_links.txt
+-rw-rw-r--   0 jake      (1000) jake      (1000)       44 2022-07-09 21:58:23.000000 chill-0.9.0/src/chill.egg-info/entry_points.txt
+-rw-rw-r--   0 jake      (1000) jake      (1000)        1 2022-01-31 13:13:57.000000 chill-0.9.0/src/chill.egg-info/not-zip-safe
+-rw-rw-r--   0 jake      (1000) jake      (1000)      121 2022-07-09 21:58:23.000000 chill-0.9.0/src/chill.egg-info/requires.txt
+-rw-rw-r--   0 jake      (1000) jake      (1000)        6 2022-07-09 21:58:23.000000 chill-0.9.0/src/chill.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chill-0.8.1/README.md` & `chill-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-[![Build Status](https://travis-ci.org/jkenlooper/chill.svg?branch=mustached-rival)](https://travis-ci.org/jkenlooper/chill)
-
 # Cascading, Highly Irrelevant, Lost Llamas
 
 *Or, just chill.*  This is a **database driven web application framework in
 [Flask](https://palletsprojects.com/p/flask/)** and it can be used to create
 static or dynamic web sites.
 
 This involves creating custom SQL queries to pull data from a database and uses
@@ -17,39 +15,44 @@
 other database queries and can recursively call other queries when populating
 the page.
 
 ## Installing
 
 Chill can be installed via pip.
 ```bash
-pip install chill
+python3 -m pip install chill
 ```
 
 Or from within this cloned project; install with pip in editable mode.  It is
-recommended to setup a virtual environment first with `virtualenv . -p python3`
-command.
+recommended to setup a virtual environment first.
+
 ```bash
-pip install -e .
+# Create a python virtual environment in the project directory and activate it.
+python3 -m venv .
+source ./bin/activate
+
+# Install chill in editable mode
+python3 -m pip install -e .
 ```
 
 This will create a script called `chill`.  Type `chill --help` for help on using
 it.  It will need a config file and such.  I recommend creating an empty
 directory and running `chill init` within it.  That will create a `site.cfg`
 config file and the bare minimum to show a homepage.  Run the 
 `chill run --config site.cfg` 
-and visit http://localhost:5000 with your browser.
+and visit http://localhost:5000/ with your browser.
 
 ## Quick start
 
 Run the `chill init` script in an empty directory and it will create a minimal
 starting point for using Chill. The `site.cfg` created will have comments on each
 configuration value.  The `chill run --config site.cfg` will run the app in the
 foreground at the http://localhost:5000/ URL. Notice that the script also
-creates a sqlite database in that directory.  This database is what the script
-uses to display the pages in a site.
+creates a sqlite database file (default file name is 'db') in that directory.
+This database file is what chill uses to display the pages in a site.
 
 **Review the docs for more.** Some helpful guides and such are in the
 [docs/](docs/) folder.  The [tests.py](src/chill/tests.py) file within the chill
 package is also a good resource.
 
 ## Static site generator
 
@@ -64,17 +67,23 @@
 * [Puzzle Massive](http://puzzle.massive.xyz/) - 
     Massively Multiplayer Online Jigsaw Puzzles
 * [Web of Tomorrow](http://www.weboftomorrow.com/) -
     A web developer's website about web development
 * [Awesome Mud Works](http://awesomemudworks.com/) -
     Pottery studio in Salt Lake City, Utah
 
-A cookiecutter for making a _chill_ website also exists.  Checkout the
-[cookiecutter-website](https://github.com/jkenlooper/cookiecutter-website/)
-project to get started.
-
 ## Docker
 
 I've included a `Dockerfile` which can be used when creating a container for
 chill.  See the 
 [guide on using chill with docker](docs/docker-container-usage.md).
 
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[GNU Lesser General Public License v3.0](https://choosealicense.com/licenses/lgpl-3.0/)
```

### Comparing `chill-0.8.1/setup.py` & `chill-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 # https://packaging.python.org/en/latest/distributing.html
 from setuptools import setup, find_packages
+import pathlib
 
-__version__ = "0.8.1"  # Also set in src/chill/_version.py
+
+here = pathlib.Path(__file__).parent.resolve()
+__version__ = "0.9.0"  # Also set in src/chill/_version.py
+long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name="chill",
     version=__version__,
     author="Jake Hickenlooper",
     author_email="jake@weboftomorrow.com",
-    keywords="static website SQL sqlite Flask web framework",
+    keywords="static website generator SQL sqlite Flask web framework",
     description="Database driven web application framework in Flask",
-    long_description="""
-        This involves creating custom SQL queries to pull your data from your database
-        into your jinja2 HTML templates for your website.  Chill creates a static
-        version of the website or can run as a Flask app. Their are a few tables that
-        are specific to Chill in order to handle page routes and what SQL query should
-        be used and such.
-    """,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url="https://github.com/jkenlooper/chill",
-    license="GPL",
+    license="LGPLv3+",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Framework :: Flask",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Internet :: WWW/HTTP :: Site Management",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
         "Topic :: Software Development :: Build Tools",
     ],
     package_dir={"": "src"},
     packages=find_packages("src"),
     package_data={"chill": ["queries/*.sql"]},
     zip_safe=False,
     test_suite="chill.tests",
     install_requires=[
-        "setuptools",
-        "docutils",
-        "Flask",
-        "Jinja2",
-        "Flask-Caching",
-        "Frozen-Flask",
-        "Flask-Markdown",
-        "future",
-        #"psycopg2", # Might switch to postgres in the future
-        "sqlalchemy",
+        "Flask>=2,<3",
+        "Jinja2>=3",
+        "Frozen-Flask==0.18",
+        "Flask-Markdown==0.3",
         "PyYAML",
         "gevent",
-        "docopt",
-        #'pyselect', # Using pyselect within src/chill/ instead
-        "MarkupSafe",
+        "docopt==0.6.2",
+        "MarkupSafe>=2,<3",
         "babel",
+        "humanize",
     ],
+    python_requires='>=3.8, <4',
     entry_points={"console_scripts": ["chill = chill.script:main"]},
 )
```

### Comparing `chill-0.8.1/src/chill/api.py` & `chill-0.9.0/src/chill/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from __future__ import absolute_import
-from sqlalchemy.exc import DatabaseError, StatementError
-from sqlalchemy.sql import text
+import sqlite3
+
 from flask import current_app, render_template
 
-from chill.app import db
-from .database import fetch_query_string, rowify
+from chill.database import get_db, fetch_query_string, serialize_sqlite3_results, ChillDBNotWritableError
+
 
 def _short_circuit(value=None):
     """
     Add the `value` to the `collection` by modifying the collection to be
     either a dict or list depending on what is already in the collection and
     value.
     Returns the collection with the value added to it.
 
     Clean up by removing single item array and single key dict.
     ['abc'] -> 'abc'
     [['abc']] -> 'abc'
+    [{'abc':123}] -> {'abc':123}
+    [[{'abc':123}]] -> {'abc':123}
     [{'abc':123},{'def':456}] -> {'abc':123,'def':456}
     [{'abc':123},{'abc':456}] -> [{'abc':123},{'abc':456}] # skip for same set keys
     [[{'abc':123},{'abc':456}]] -> [{'abc':123},{'abc':456}]
     """
     if not isinstance(value, list):
         return value
     if len(value) == 0:
@@ -46,110 +47,158 @@
                 return newvalue
             else:
                 return value
         else:
             return value
 
 
-
 def _query(_node_id, value=None, **kw):
     "Look up value by using Query table"
+    # GET query method can only be read
+    # POST query method can be read or write
+    if current_app.config.get("database_readonly") and kw["method"] in ("PUT", "PATCH", "DELETE"):
+        raise Exception("Database is currently readonly, but started processing a query method that was not readonly")
     query_result = []
+    db = get_db()
+    cur = db.cursor()
     try:
-        query_result = db.execute(text(fetch_query_string('select_query_from_node.sql')), **kw).fetchall()
-    except DatabaseError as err:
+        query_result = cur.execute(
+            fetch_query_string("select_query_from_node.sql"), kw
+        ).fetchall()
+    except sqlite3.DatabaseError as err:
         current_app.logger.error("DatabaseError: %s, %s", err, kw)
+        cur.close()
         return value
-    #current_app.logger.debug("queries kw: %s", kw)
-    #current_app.logger.debug("queries value: %s", value)
-    #current_app.logger.debug("queries: %s", query_result)
+    # current_app.logger.debug("queries kw: %s", kw)
+    # current_app.logger.debug("queries value: %s", value)
+    # current_app.logger.debug("queries: %s", serialize_sqlite3_results(query_result))
+    ignored_db_error = False
     if query_result:
         values = []
-        for query_name in [x['name'] for x in query_result]:
+        for query_name in [x["name"] for x in query_result]:
             if query_name:
                 result = []
                 try:
-                    #current_app.logger.debug("query_name: %s", query_name)
-                    #current_app.logger.debug("kw: %s", kw)
+                    current_app.logger.debug("query_name: %s", query_name)
+                    current_app.logger.debug("kw: %s", kw)
                     # Query string can be insert or select here
-                    #statement = text(fetch_query_string(query_name))
-                    #params = [x.key for x in statement.params().get_children()]
-                    #skw = {key: kw[key] for key in params}
-                    #result = db.execute(statement, **skw)
-                    result = db.execute(text(fetch_query_string(query_name)), **kw)
-                    #current_app.logger.debug("result query: %s", list(result.keys()))
-                except (DatabaseError, StatementError) as err:
-                    current_app.logger.error("DatabaseError (%s) %s: %s", query_name, kw, err)
-                if result and result.returns_rows:
+                    # statement = fetch_query_string(query_name)
+                    # params = [x.key for x in statement.params().get_children()]
+                    # skw = {key: kw[key] for key in params}
+                    # result = cur.execute(statement, **skw)
+                    result = cur.execute(fetch_query_string(query_name), kw)
+                except (sqlite3.DatabaseError, sqlite3.ProgrammingError) as err:
+                    ignored_db_error = True
+                    current_app.logger.error(
+                        "DatabaseError (%s) %s: %s", query_name, kw, err
+                    )
+                if result:
                     result = result.fetchall()
-                    #values.append(([[dict(zip(result.keys(), x)) for x in result]], result.keys()))
-                    #values.append((result.fetchall(), result.keys()))
-                    #current_app.logger.debug("fetchall: %s", values)
+                    # values.append(([[dict(zip(result.keys(), x)) for x in result]], result.keys()))
+                    # values.append((result.fetchall(), result.keys()))
+                    # current_app.logger.debug("fetchall: %s", values)
                     if len(result) == 0:
-                        values.append(([], []))
+                        current_app.logger.debug("result is empty")
+                        # values.append([{}])
+                        values.append([{}])
                     else:
-                        #current_app.logger.debug("result: %s", result)
-                        # There may be more results, but only interested in the
-                        # first one. Use the older rowify method for now.
-                        # TODO: use case for rowify?
-                        values.append(rowify(result, [(x, None) for x in list(result[0].keys())]))
-                        #current_app.logger.debug("fetchone: %s", values)
+                        current_app.logger.debug(
+                            "result: %s", serialize_sqlite3_results(result)
+                        )
+                        values.append(result)
         value = values
-    #current_app.logger.debug("value: %s", value)
+    # current_app.logger.debug("value: %s", value)
+    cur.close()
+
+    if kw["method"] == "GET" and db.in_transaction:
+        raise Exception("There are uncommitted changes to db when query was GET")
+    if kw["method"] == "POST" and (db.in_transaction or ignored_db_error) and current_app.config.get("database_readonly"):
+        if db.in_transaction:
+            current_app.logger.error("There are uncommitted changes to read only db connection when query was POST")
+            raise ChillDBNotWritableError("There are uncommitted changes to read only db connection when query was POST")
+        elif ignored_db_error:
+            current_app.logger.error("There were database query errors to read only db connection when query was POST")
+            raise ChillDBNotWritableError("There were database query errors to read only db connection when query was POST")
+        else:
+            raise Exception("Not handled error.")
+    if current_app.config.get("database_readonly") and db.in_transaction:
+        current_app.logger.error("There are uncommitted changes to db when query should have been readonly")
+        raise Exception("There are uncommitted changes to db when query should have been readonly")
+    if not current_app.config.get("database_readonly"):
+        # Only need to commit a transaction if the database is not in read only
+        # mode.
+        db.commit()
+
     return value
 
+
 def _template(node_id, value=None):
     "Check if a template is assigned to it and render that with the value"
+    db = get_db()
+    if value:
+        value = serialize_sqlite3_results(value)
     result = []
-    select_template_from_node = fetch_query_string('select_template_from_node.sql')
+    select_template_from_node = fetch_query_string("select_template_from_node.sql")
+    cur = db.cursor()
     try:
-        result = db.execute(text(select_template_from_node), node_id=node_id)
+        result = cur.execute(select_template_from_node, {"node_id": node_id})
         template_result = result.fetchone()
-        result.close()
-        if template_result and template_result['name']:
-            template = template_result['name']
+        cur.close()
+        if template_result and template_result["name"]:
+            template = template_result["name"]
 
             if isinstance(value, dict):
                 return render_template(template, **value)
             else:
                 return render_template(template, value=value)
-    except DatabaseError as err:
+    except sqlite3.DatabaseError as err:
         current_app.logger.error("DatabaseError: %s", err)
 
     # No template assigned to this node so just return the value
     return value
 
+
 def render_node(_node_id, value=None, noderequest={}, **kw):
     "Recursively render a node's value"
-    if value == None:
-        kw.update( noderequest )
+    if value is None:
+        kw.update(noderequest)
+        kw["method"] = "GET"
         results = _query(_node_id, **kw)
-        #current_app.logger.debug("results: %s", results)
+        current_app.logger.debug("render_node results: %s", results)
         if results:
             values = []
-            for (result, cols) in results:
-                if set(cols) == set(['node_id', 'name', 'value']):
+            for result in results:
+                if set(result[0].keys()) == set(["node_id", "name", "value"]):
                     for subresult in result:
-                        #if subresult.get('name') == kw.get('name'):
-                            # This is a link node
-                        #current_app.logger.debug("sub: %s", subresult)
-                        name = subresult['name']
-                        if noderequest.get('_no_template'):
-                            # For debugging or just simply viewing with the
-                            # operate script we append the node_id to the name
+                        # if subresult.get('name') == kw.get('name'):
+                        # This is a link node
+                        current_app.logger.debug("sub: %s", subresult)
+                        name = subresult["name"]
+                        if noderequest.get("_no_template"):
+                            # For debugging; append the node_id to the name
                             # of each. This doesn't work with templates.
-                            name = "{0} ({1})".format(name, subresult['node_id'])
-                        values.append( {name: render_node( subresult['node_id'], noderequest=noderequest, **subresult )} )
-                #elif 'node_id' and 'name' in cols:
+                            name = "{0} ({1})".format(name, subresult["node_id"])
+                        values.append(
+                            {
+                                name: render_node(
+                                    subresult["node_id"],
+                                    noderequest=noderequest,
+                                    **subresult
+                                )
+                            }
+                        )
+                # elif 'node_id' and 'name' in cols:
                 #    for subresult in result:
                 #        current_app.logger.debug("sub2: %s", subresult)
                 #        values.append( {subresult.get('name'): render_node( subresult.get('node_id'), **subresult )} )
                 else:
-                    values.append( result )
+                    values.append(result)
 
             value = values
 
     value = _short_circuit(value)
-    if not noderequest.get('_no_template'):
+    # current_app.logger.debug(f"after sc: {value}")
+    if not noderequest.get("_no_template"):
         value = _template(_node_id, value)
+        # current_app.logger.debug(f"after template: {value}")
 
     return value
```

### Comparing `chill-0.8.1/src/chill/app.py` & `chill-0.9.0/src/chill/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-from __future__ import absolute_import
-from builtins import str, bytes
 import os
 import time
-import sqlite3
 
-from werkzeug.local import LocalProxy
-from flask import Flask, g, current_app, Blueprint, Markup
+from flask import Flask, Blueprint, Markup
 from flask.helpers import send_from_directory
 from flaskext.markdown import Markdown
 from jinja2 import FileSystemLoader
-from .cache import cache
-from sqlalchemy import create_engine
-from sqlalchemy.engine import Engine
-from sqlalchemy import event
 from babel import dates
+from humanize import naturaltime
 
-from . import shortcodes
-
-# from chill.resource import resource
-# from chill.page import page
+from chill import shortcodes
+from chill import database
 
 
 class ChillFlask(Flask):
     def send_root_file(self, filename):
         """
         Function used to send static files from the root of the domain.
         """
@@ -46,54 +37,14 @@
         """
         cache_timeout = self.get_send_file_max_age(filename)
         return send_from_directory(
             self.config["THEME_STATIC_FOLDER"], filename, cache_timeout=cache_timeout
         )
 
 
-def connect_to_database():
-    """
-    Return the engine. Echo all sql statements if in DEBUG mode.
-    """
-    def sqlite_readonly_connect():
-
-        db_file = current_app.config.get("CHILL_DATABASE_URI")[len('sqlite:///'):]
-        if db_file and not db_file.startswith(':'):
-            # Open the database connection in read only mode
-            return sqlite3.connect(
-                "file:{}?mode=ro".format(db_file), uri=True
-            )
-        else:
-            return sqlite3.connect(current_app.config.get("CHILL_DATABASE_URI"))
-
-    if current_app.config.get("database_readonly") and current_app.config.get("is_sqlite_database"):
-        return create_engine(current_app.config["CHILL_DATABASE_URI"], creator=sqlite_readonly_connect)
-    else:
-        return create_engine(current_app.config["CHILL_DATABASE_URI"])
-
-
-def get_db():
-    db = getattr(g, "_database", None)
-    if db is None:
-        db = g._database = connect_to_database()
-        if str(db.url).startswith("sqlite://"):
-            # Enable foreign key support so 'on update' and 'on delete' actions
-            # will apply. This needs to be set for each db connection.
-            @event.listens_for(Engine, "connect")
-            def set_sqlite_pragma(dbapi_connection, connection_record):
-                cursor = dbapi_connection.cursor()
-                cursor.execute("PRAGMA foreign_keys=ON")
-                cursor.close()
-
-    return db
-
-
-db = LocalProxy(get_db)
-
-
 def multiple_directory_files_loader(*args):
     """
     Loads all the files in each directory as values in a dict with the key
     being the relative file path of the directory.  Updates the value if
     subsequent file paths are the same.
     """
     d = dict()
@@ -120,18 +71,14 @@
 
     if config:
         config_file = (
             config if config[0] == os.sep else os.path.join(os.getcwd(), config)
         )
         app.config.from_pyfile(config_file)
     app.config.update(kw, database_readonly=database_readonly)
-    is_sqlite_database = str(app.config.get("CHILL_DATABASE_URI")).startswith("sqlite://")
-    app.config["is_sqlite_database"] = is_sqlite_database
-
-    cache.init_app(app)
 
     # Set the freezer destination path to be absolute if needed.
     freeze_folder = app.config.get("FREEZER_DESTINATION", None)
     if freeze_folder:
         if freeze_folder[0] != os.sep:
             freeze_folder = os.path.join(os.getcwd(), freeze_folder)
 
@@ -185,19 +132,16 @@
     app.queries = multiple_directory_files_loader(
         chill_queries_folder, user_queries_folder
     )
 
     # Set the jinja2 template folder eith fallback for app.template_folder
     app.jinja_env.loader = FileSystemLoader(app.config.get("THEME_TEMPLATE_FOLDER"))
 
-    @app.teardown_appcontext
-    def teardown_db(exception):
-        db = getattr(g, "_database", None)
-        if db is not None:
-            db.dispose()
+    app.logger.debug("Database init_app")
+    database.init_app(app)
 
     # STATIC_URL='http://cdn.example.com/whatever/works/'
     @app.context_processor
     def inject_paths():
         """
         Inject the variables 'theme_static_path' and 'media_path' into the templates.
 
@@ -230,19 +174,20 @@
     @app.template_filter("datetime")
     def datetime(value, format="y-MM-dd HH:mm:ss"):
         "Date time filter that uses babel to format."
         return dates.format_datetime(value, format)
 
     @app.template_filter("timedelta")
     def timedelta(value):
-        "time delta"
-        return dates.format_timedelta(value)
+        "time delta using humanize.time.naturaltime()"
+        return naturaltime(value)
 
     # Add the markdown filter for the templates
-    md = Markdown(app)
+    # https://pythonhosted.org/Flask-Markdown/
+    Markdown(app)
 
     @app.template_filter("readfile")
     def readfile(filename):
         "A template filter to read files from the DOCUMENT_FOLDER"
         document_folder = app.config.get("DOCUMENT_FOLDER")
         if document_folder:
             # Restrict access to just the DOCUMENT_FOLDER.
@@ -261,17 +206,22 @@
 
                 # py3 (not py2 compat)
                 # content = f.read()
 
                 # py2 and py3 compat
                 content = bytes(f.read(), "utf-8").decode("utf-8")
             return content
+        else:
+            app.logger.warning(
+                "The DOCUMENT_FOLDER setting in site.cfg is not set to a value. Can't use 'readfile' filter."
+            )
+            return filename
 
         app.logger.warn(
-            "jinja2 filter 'readfile' can't find file: '{0}'".format(filename)
+            f"jinja2 filter 'readfile' can't find file: '{filename}' at DOCUMENT_FOLDER path: {document_folder}"
         )
         return filename
 
     # register any blueprints here
     # app.logger.warning("Not registering resource blueprint")
     # app.register_blueprint(resource)
```

### Comparing `chill-0.8.1/src/chill/migrations.py` & `chill-0.9.0/src/chill/migrations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,93 @@
 import sqlite3
 from flask import current_app
-from chill.app import make_app, db
 from chill.database import (
-        fetch_query_string,
-        rowify,
-        )
+    get_db,
+    fetch_query_string,
+)
 
 
 def migrate1():
     "Migrate from version 0 to 1"
 
     initial = [
-    "create table Chill (version integer);",
-    "insert into Chill (version) values (1);",
-    "alter table SelectSQL rename to Query;",
-    "alter table Node add column template integer references Template (id) on delete set null;",
-    "alter table Node add column query integer references Query (id) on delete set null;"
+        "create table Chill (version integer);",
+        "insert into Chill (version) values (1);",
+        "alter table SelectSQL rename to Query;",
+        "alter table Node add column template integer references Template (id) on delete set null;",
+        "alter table Node add column query integer references Query (id) on delete set null;",
     ]
 
+    cleanup = ["drop table SelectSQL_Node;", "drop table Template_Node;"]
 
-    cleanup = [
-    "drop table SelectSQL_Node;",
-    "drop table Template_Node;"
-    ]
-
-    c = db.cursor()
+    db = get_db()
+    cur = db.cursor()
     try:
-        c.execute("select version from Chill limit 1;")
+        cur.execute("select version from Chill limit 1;")
     except sqlite3.DatabaseError as err:
         pass
-    result = c.fetchone()
+    result = cur.fetchone()
     if result:
         version = result[0]
         if version == 1:
             current_app.logger.warn("Migration from version 0 to 1 is not needed.")
         else:
-            current_app.logger.warn("Migration from version 0 to {0} is not supported.".format(version))
+            current_app.logger.warn(
+                "Migration from version 0 to {0} is not supported.".format(version)
+            )
+        cur.close()
         return
 
-    try:
-        for query in initial:
-            c.execute(query)
-    except sqlite3.DatabaseError as err:
-        current_app.logger.error("DatabaseError: %s", err)
-
-    try:
-        c.execute(fetch_query_string('select_all_nodes.sql'))
-    except sqlite3.DatabaseError as err:
-        current_app.logger.error("DatabaseError: %s", err)
-    result = c.fetchall()
-    if result:
-        (result, col_names) = rowify(result, c.description)
-        for kw in result:
+    with db:
+        try:
+            for query in initial:
+                cur.execute(query)
+        except sqlite3.DatabaseError as err:
+            current_app.logger.error("DatabaseError: %s", err)
 
-            try:
-                c.execute("""
-                update Node set template = (
-                select t.id from Template as t
-                join Template_Node as tn on ( tn.template_id = t.id )
-                join Node as n on ( n.id = tn.node_id )
-                where n.id is :node_id
-                group by t.id)
-                where id is :node_id;
-                """, {'node_id':kw['id']})
-            except sqlite3.DatabaseError as err:
-                current_app.logger.error("DatabaseError: %s", err)
-
-            try:
-                c.execute("""
-                update Node set query = (
-                select s.id from Query as s
-                join SelectSQL_Node as sn on ( sn.selectsql_id = s.id )
-                join Node as n on ( n.id = sn.node_id )
-                where n.id is :node_id
-                group by s.id)
-                where id is :node_id;
-                """, {'node_id':kw['id']})
-            except sqlite3.DatabaseError as err:
-                current_app.logger.error("DatabaseError: %s", err)
     try:
-        for query in cleanup:
-            c.execute(query)
+        cur.execute(fetch_query_string("select_all_nodes.sql"))
     except sqlite3.DatabaseError as err:
         current_app.logger.error("DatabaseError: %s", err)
+    result = cur.fetchall()
+    with db:
+        if result:
+            for kw in result:
+
+                try:
+                    cur.execute(
+                        """
+                    update Node set template = (
+                    select t.id from Template as t
+                    join Template_Node as tn on ( tn.template_id = t.id )
+                    join Node as n on ( n.id = tn.node_id )
+                    where n.id is :node_id
+                    group by t.id)
+                    where id is :node_id;
+                    """,
+                        {"node_id": kw["id"]},
+                    )
+                except sqlite3.DatabaseError as err:
+                    current_app.logger.error("DatabaseError: %s", err)
+
+                try:
+                    cur.execute(
+                        """
+                    update Node set query = (
+                    select s.id from Query as s
+                    join SelectSQL_Node as sn on ( sn.selectsql_id = s.id )
+                    join Node as n on ( n.id = sn.node_id )
+                    where n.id is :node_id
+                    group by s.id)
+                    where id is :node_id;
+                    """,
+                        {"node_id": kw["id"]},
+                    )
+                except sqlite3.DatabaseError as err:
+                    current_app.logger.error("DatabaseError: %s", err)
+        try:
+            for query in cleanup:
+                cur.execute(query)
+        except sqlite3.DatabaseError as err:
+            current_app.logger.error("DatabaseError: %s", err)
 
-    db.commit()
+        cur.close()
```

### Comparing `chill-0.8.1/src/chill/public.py` & `chill-0.9.0/src/chill/public.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,299 +1,365 @@
-from __future__ import absolute_import
-from builtins import str
 import os
 import os.path
+import sqlite3
 
-from sqlalchemy.sql import text
-from sqlalchemy.exc import (
-        DatabaseError,
-        OperationalError
-        )
 from werkzeug.routing import Map, Rule
 from werkzeug.exceptions import HTTPException
 
 from flask import (
-        abort, redirect, Blueprint, current_app, render_template, json, request, make_response, app,
-        url_for
-        )
+    abort,
+    current_app,
+    json,
+    request,
+    make_response,
+    url_for,
+)
 from flask.views import MethodView
 
-from chill.app import db
-from .database import fetch_query_string, rowify
-from .api import render_node, _query
-from .cache import cache
-from . import shortcodes
+from chill.database import get_db, fetch_query_string, serialize_sqlite3_results, ChillDBNotWritableError
+from chill.api import render_node, _query, _short_circuit
+from chill import shortcodes
 
-#def get_map_adapter():
+
+# def get_map_adapter():
 #    map_adapter = getattr(
 #
 def check_map(uri, url_root):
     """
     return a tuple of the rule and kw.
     """
     # TODO: Building the Map each time this is called seems like it could be more effiecent.
     result = []
+    db = get_db()
     try:
-        result = db.execute(text(fetch_query_string('select_route_where_dynamic.sql'))).fetchall()
-    except OperationalError as err:
+        cur = db.cursor()
+        result = cur.execute(
+            fetch_query_string("select_route_where_dynamic.sql")
+        ).fetchall()
+        cur.close()
+    except sqlite3.OperationalError as err:
         current_app.logger.error("OperationalError: %s", err)
+        cur.close()
         return (None, None)
     if result:
-        #routes = result.as_dict()
-        #(routes, col_names) = rowify(result, c.description)
-        #current_app.logger.debug( [x['rule'] for x in routes] )
-        rules = [Rule(r['rule'], endpoint='dynamic') for r in result]
-        d_map = Map( rules )
+        # routes = result.as_dict()
+        # (routes, col_names) = rowify(result, c.description)
+        # current_app.logger.debug( [x['rule'] for x in routes] )
+        rules = [Rule(r["rule"], endpoint="dynamic") for r in result]
+        d_map = Map(rules)
         map_adapter = d_map.bind(url_root)
-        #current_app.logger.debug(uri)
+        # current_app.logger.debug(uri)
         try:
             (rule, rule_kw) = map_adapter.match(path_info=uri, return_rule=True)
-            #current_app.logger.debug(rule)
+            # current_app.logger.debug(rule)
             return (str(rule), rule_kw)
         except HTTPException:
             pass
     return (None, {})
 
+
 def node_from_uri(uri, method="GET"):
     # check if page exists in data_path
 
     # a//b == a/b/ == a/./b == a/foo/../b
     # '' == '.'
     # Prepend the uri with '/' and normalize
-    uri = os.path.normpath(os.path.join('/', uri))
+    uri = os.path.normpath(os.path.join("/", uri))
 
     uri, ext = os.path.splitext(uri)
-    if not uri.endswith('/'):
-        uri = ''.join((uri, '/'))
+    if not uri.endswith("/"):
+        uri = "".join((uri, "/"))
 
-    #current_app.logger.debug('uri: "%s"' % uri)
+    # current_app.logger.debug('uri: "%s"' % uri)
 
     rule_kw = {}
-    select_node_from_route = fetch_query_string('select_node_from_route.sql')
+    select_node_from_route = fetch_query_string("select_node_from_route.sql")
 
-    result = []
+    result = None
+    db = get_db()
+    cur = db.cursor()
     try:
-        result = db.execute(text(select_node_from_route), uri=uri, method=method).fetchall()
-    except DatabaseError as err:
+        result = cur.execute(
+            select_node_from_route, {"uri": uri, "method": method}
+        ).fetchone()
+    except sqlite3.DatabaseError as err:
         current_app.logger.error("DatabaseError: %s", err)
 
-    #current_app.logger.debug('result: "{}", {}'.format(result, len(result)))
-    if not result or len(result) == 0:
+    # current_app.logger.debug('result: "{}", {}'.format(result, len(result)))
+    if not result:
         # See if the uri matches any dynamic rules
         (rule, rule_kw) = check_map(uri, request.url_root)
-        #current_app.logger.debug(rule)
-        #current_app.logger.debug('rule: "%s"' % rule or '')
+        # current_app.logger.debug(rule)
+        # current_app.logger.debug('rule: "%s"' % rule or '')
         if rule:
             try:
-                result = db.execute(text(select_node_from_route), uri=rule, method=method).fetchall()
-            except DatabaseError as err:
+                # Only one result for a getting a node from a unique path.
+                result = cur.execute(
+                    select_node_from_route, {"uri": rule, "method": method}
+                ).fetchone()
+            except sqlite3.DatabaseError as err:
                 current_app.logger.error("DatabaseError: %s", err)
 
-    if result:
-        #result = result.as_dict()
-        #(result, col_names) = rowify(result, c.description)
-
-        # Only one result for a getting a node from a unique path.
-        return (result[0], rule_kw)
-    return (None, rule_kw)
-
-def skip_cache():
-    """Skip the cache if request has Chill-Skip-Cache set"""
-    if u'Chill-Skip-Cache' in request.headers:
-        return True
+    cur.close()
+    return (result, rule_kw)
 
-    return False
 
 # The page blueprint has no static files or templates read from disk.
-#page = Blueprint('public', __name__, static_folder=os.path.join( os.getcwd(), current_app.config.get('CHILL_STATIC_DIR', 'static') ), template_folder=None)
+# page = Blueprint('public', __name__, static_folder=os.path.join( os.getcwd(), current_app.config.get('CHILL_STATIC_DIR', 'static') ), template_folder=None)
+
+# page.record(set_map)
+# map_adapter = map.bind('example.com')
 
-#page.record(set_map)
-#map_adapter = map.bind('example.com')
 
 class PageView(MethodView):
     """
     Handles access to a uri.
     The uri is first matched directly with a route to get a node. If that
     fails, it will load up the custom map and check the uri with any matching
     routes.
 
     When a node is retrieved (get) it renders that nodes value. (See `render_node`.)
     """
 
-    @cache.cached(unless=skip_cache)
-    def get(self, uri=''):
+    def get(self, uri=""):
         "For sql queries that start with 'SELECT ...'"
         (node, rule_kw) = node_from_uri(uri)
 
-        if node == None:
+        if node is None:
             abort(404)
-        rule_kw.update( node )
+
+        rule_kw.update(node)
         values = rule_kw
+        if "method" in values.keys():
+            abort(500)
+
         xhr_data = request.get_json(silent=True)
         if xhr_data:
-            values.update( xhr_data )
-        values.update( request.form.to_dict(flat=True) )
-        values.update( request.args.to_dict(flat=True) )
-        values.update( request.cookies )
-        values['method'] = request.method
+            values.update(xhr_data)
+        values.update(request.form.to_dict(flat=True))
+        values.update(request.args.to_dict(flat=True))
+        values.update(request.cookies)
+        if "method" in values.keys():
+            abort(400)
+
+        values["method"] = request.method
         noderequest = values.copy()
-        noderequest.pop('node_id')
-        noderequest.pop('name')
-        noderequest.pop('value')
-
-        #current_app.logger.debug("get kw: %s", values)
-        rendered = render_node(node['id'], noderequest=noderequest, **values)
-        #current_app.logger.debug("rendered: %s", rendered)
+        noderequest.pop("node_id")
+        noderequest.pop("name")
+        noderequest.pop("value")
+
+        # current_app.logger.debug("get kw: %s", values)
+        rendered = render_node(node["id"], noderequest=noderequest, **values)
+        # current_app.logger.debug("rendered: %s", rendered)
         if rendered:
-            if not isinstance(rendered, (str, str, int, float)):
+            if not isinstance(rendered, (str, int, float)):
                 # return a json string
-                return json.jsonify(rendered)
+                return json.jsonify(serialize_sqlite3_results(rendered))
             return rendered
 
         # Nothing to show, so nothing found
         abort(404)
 
-
-    def post(self, uri=''):
-        "For sql queries that start with 'INSERT ...'"
+    def post(self, uri=""):
+        "For sql queries that start with 'SELECT ...' or 'INSERT ...'"
 
         # get node...
         (node, rule_kw) = node_from_uri(uri, method=request.method)
-        if node == None:
+        if node is None:
             abort(404)
 
-        rule_kw.update( node )
+        rule_kw.update(node)
         values = rule_kw
+        if "method" in values.keys():
+            abort(500)
         xhr_data = request.get_json(silent=True)
         if xhr_data:
-            values.update( xhr_data )
-        values.update( request.form.to_dict(flat=True) )
-        values.update( request.args.to_dict(flat=True) )
-        values['method'] = request.method
+            values.update(xhr_data)
+        values.update(request.form.to_dict(flat=True))
+        values.update(request.args.to_dict(flat=True))
+
+        if "method" in values.keys():
+            abort(400)
+        values["method"] = request.method
 
         # Execute the sql query with the data
-        _query(node['id'], **values)
+        try:
+            query_result = _query(node["id"], **values)
+        except (ChillDBNotWritableError):
+            current_app.logger.warning(
+                f"Can't handle {request.method} request method for {uri} when database is read only"
+            )
+            abort(400)
+
+        # A POST can return a response in case it is used like a GET method.  An
+        # example would be for a complex search query.
+        if query_result and query_result != [[{}]]:
+            query_result = _short_circuit(query_result)
+            if not isinstance(query_result, (str, int, float)):
+                # return a json string
+                return json.jsonify(serialize_sqlite3_results(query_result))
+            return query_result
+
+        else:
+            response = make_response("ok", 201)
 
-        response = make_response('ok', 201)
         return response
 
-    def put(self, uri=''):
+    def put(self, uri=""):
         "For sql queries that start with 'INSERT ...' or 'UPDATE ...'"
 
+        if current_app.config.get("database_readonly"):
+            current_app.logger.warning(
+                f"Can't handle {request.method} request method for {uri} when database is read only"
+            )
+            abort(400)
+
         # get node...
         (node, rule_kw) = node_from_uri(uri, method=request.method)
-        if node == None:
+        if node is None:
             abort(404)
 
-        rule_kw.update( node )
+        rule_kw.update(node)
         values = rule_kw
+        if "method" in values.keys():
+            abort(500)
+
         xhr_data = request.get_json(silent=True)
         if xhr_data:
-            values.update( xhr_data )
-        values.update( request.form.to_dict(flat=True) )
-        values.update( request.args.to_dict(flat=True) )
-        values['method'] = request.method
+            values.update(xhr_data)
+        values.update(request.form.to_dict(flat=True))
+        values.update(request.args.to_dict(flat=True))
+
+        if "method" in values.keys():
+            abort(400)
+        values["method"] = request.method
 
         # Execute the sql query with the data
-        _query(node['id'], **values)
+        _query(node["id"], **values)
 
-        response = make_response('ok', 201)
+        response = make_response("ok", 201)
         return response
 
-    def patch(self, uri=''):
+    def patch(self, uri=""):
         "For sql queries that start with 'UPDATE ...'"
 
+        if current_app.config.get("database_readonly"):
+            current_app.logger.warning(
+                f"Can't handle {request.method} request method for {uri} when database is read only"
+            )
+            abort(400)
+
         # get node...
         (node, rule_kw) = node_from_uri(uri, method=request.method)
-        if node == None:
+        if node is None:
             abort(404)
 
-        rule_kw.update( node )
+        rule_kw.update(node)
         values = rule_kw
+        if "method" in values.keys():
+            abort(500)
+
         xhr_data = request.get_json(silent=True)
         if xhr_data:
-            values.update( xhr_data )
-        values.update( request.form.to_dict(flat=True) )
-        values.update( request.args.to_dict(flat=True) )
-        values['method'] = request.method
+            values.update(xhr_data)
+        values.update(request.form.to_dict(flat=True))
+        values.update(request.args.to_dict(flat=True))
+
+        if "method" in values.keys():
+            abort(400)
+        values["method"] = request.method
 
         # Execute the sql query with the data
-        _query(node['id'], **values)
+        _query(node["id"], **values)
 
-        response = make_response('ok', 201)
+        response = make_response("ok", 201)
         return response
 
-    def delete(self, uri=''):
+    def delete(self, uri=""):
         "For sql queries that start with 'DELETE from ...'"
 
+        if current_app.config.get("database_readonly"):
+            current_app.logger.warning(
+                f"Can't handle {request.method} request method for {uri} when database is read only"
+            )
+            abort(400)
+
         # get node...
         (node, rule_kw) = node_from_uri(uri, method=request.method)
-        if node == None:
+        if node is None:
             abort(404)
 
-        rule_kw.update( node )
+        rule_kw.update(node)
         values = rule_kw
+        if "method" in values.keys():
+            abort(500)
+
         xhr_data = request.get_json(silent=True)
         if xhr_data:
-            values.update( xhr_data )
-        values.update( request.form.to_dict(flat=True) )
-        values.update( request.args.to_dict(flat=True) )
-        values['method'] = request.method
+            values.update(xhr_data)
+        values.update(request.form.to_dict(flat=True))
+        values.update(request.args.to_dict(flat=True))
+
+        if "method" in values.keys():
+            abort(400)
+        values["method"] = request.method
 
         # Execute the sql query with the data
-        _query(node['id'], **values)
+        _query(node["id"], **values)
 
-        response = make_response('ok', 204)
+        response = make_response("ok", 204)
         return response
 
-@shortcodes.register('route')
+
+@shortcodes.register("route")
 def route_handler(context, content, pargs, kwargs):
     """
     Route shortcode works a lot like rendering a page based on the url or
     route.  This allows inserting in rendered HTML within another page.
 
     Activate it with the 'shortcodes' template filter. Within the content use
     the chill route shortcode: "[chill route /path/to/something/]" where the
     '[chill' and ']' are the shortcode starting and ending tags. And 'route' is
     this route handler that takes one argument which is the url.
     """
     (node, rule_kw) = node_from_uri(pargs[0])
 
-    if node == None:
-        return u"<!-- 404 '{0}' -->".format(pargs[0])
+    if node is None:
+        return "<!-- 404 '{0}' -->".format(pargs[0])
 
-    rule_kw.update( node )
+    rule_kw.update(node)
     values = rule_kw
-    values.update( request.form.to_dict(flat=True) )
-    values.update( request.args.to_dict(flat=True) )
-    values['method'] = request.method
+    values.update(request.form.to_dict(flat=True))
+    values.update(request.args.to_dict(flat=True))
+    values["method"] = request.method
     noderequest = values.copy()
-    noderequest.pop('node_id')
-    noderequest.pop('name')
-    noderequest.pop('value')
+    noderequest.pop("node_id")
+    noderequest.pop("name")
+    noderequest.pop("value")
 
-    rendered = render_node(node['id'], noderequest=noderequest, **values)
+    rendered = render_node(node["id"], noderequest=noderequest, **values)
 
     if rendered:
         if not isinstance(rendered, (str, str, int, float)):
             # return a json string
             return json.jsonify(rendered)
 
         return rendered
 
     # Nothing to show, so nothing found
     return "<!-- 404 '{0}' -->".format(pargs[0])
 
-@shortcodes.register('page_uri')
+
+@shortcodes.register("page_uri")
 def page_uri_handler(context, content, pargs, kwargs):
     """
     Shortcode for getting the link to internal pages using the flask `url_for`
     method.
 
     Activate with 'shortcodes' template filter. Within the content use the
     chill page_uri shortcode: "[chill page_uri idofapage]". The argument is the
     'uri' for a page that chill uses.
 
     Does not verify the link to see if it's valid.
     """
     uri = pargs[0]
-    return url_for('.page_uri', uri=uri)
+    return url_for(".page_uri", uri=uri)
```

### Comparing `chill-0.8.1/src/chill/queries/create_picture.sql` & `chill-0.9.0/src/chill/queries/create_picture.sql`

 * *Files identical despite different names*

### Comparing `chill-0.8.1/src/chill/script.py` & `chill-0.9.0/src/chill/script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Chill - Database driven web application framework in Flask
 
 Usage: chill run [--config <file>] [--readonly]
        chill serve [--config <file>] [--readonly]
        chill freeze [--config <file>] [--urls <file>]
-       chill operate [--config <file>]
        chill init
        chill initdb [--config <file>]
+       chill dropdb [--config <file>]
        chill load [--config <file>] [--yaml <file>]
        chill dump [--config <file>] [--yaml <file>]
        chill migrate [--config <file>]
        chill --help
        chill --version
 
 Options:
@@ -20,167 +20,177 @@
   --urls <file>     A txt file with a url to freeze on each line
   --yaml <file>     A yaml file with ChillNode objects [default: ./chill-data.yaml]
 
 Subcommands:
     run     - Start the web server in the foreground. Don't use for production.
     serve   - Starts a daemon web server with Gevent.
     freeze  - Freeze the application by creating a static version of it.
-    operate - Interface to do simple operations on the database.
     init    - Initialize the current directory with base starting files and database.
     initdb  - Initialize Chill database tables only.
+    dropdb  - Deletes Chill database tables only.
     load    - Load a yaml file that has ChillNode objects into the database.
     dump    - Create a yaml file of ChillNode objects from the database.
     migrate - Perform a database migration from one version to the next.
 
 """
 from gevent import monkey
+
 monkey.patch_all()
 
-from builtins import map
 import os
 import subprocess
 import sqlite3
 
-from sqlalchemy.exc import DatabaseError, StatementError
-from sqlalchemy.sql import text
 from docopt import docopt
 from flask_frozen import Freezer
 
-from chill.app import make_app, db
+from chill.app import make_app
 from chill.database import (
+    get_db,
     init_db,
+    drop_db,
     insert_node,
     insert_node_node,
     insert_route,
     insert_query,
     add_template_for_node,
     fetch_query_string,
 )
-from chill.operate import operate_menu
 from chill.migrations import migrate1
 from chill.yaml_chill_node import load_yaml, dump_yaml
 from chill._version import __version__
 
 SITECFG = """
+from os import getenv
+from os.path import isfile
+import json
+
 # The site.cfg file is used to configure a flask app.  Refer to the flask
 # documentation for other configurations.  The below are used specifically by
 # Chill.
 
 # Set the HOST to 0.0.0.0 for being an externally visible server.
-#HOST = '127.0.0.1'
-#PORT = 5000
+# Set the HOST to 127.0.0.1 for internal
+HOST = getenv("CHILL_HOST", default="0.0.0.0")
+PORT = int(getenv("CHILL_PORT", default="5000"))
+
+# Optional if needing to freeze the site and absolute URLs are needed. See the
+# FREEZER_BASE_URL setting below.
+HOSTNAME = getenv("CHILL_HOSTNAME", default="localhost")
 
-# Valid SQLite URL forms are:
-#   sqlite:///:memory: (or, sqlite://)
-#   sqlite:///relative/path/to/file.db
-#   sqlite:////absolute/path/to/file.db
-# http://docs.sqlalchemy.org/en/latest/core/engines.html
-CHILL_DATABASE_URI = "sqlite:///db"
+# Path to sqlite3 database file
+CHILL_DATABASE_URI = getenv("CHILL_DATABASE_URI", default="db")
 
 # Set the sqlite journal_mode
 # https://sqlite.org/pragma.html#pragma_journal_mode
-# Leave blank to not change
-SQLITE_JOURNAL_MODE = ""
+SQLITE_JOURNAL_MODE = getenv("CHILL_SQLITE_JOURNAL_MODE", default="wal")
 
 # If using the ROOT_FOLDER then you will need to set the PUBLIC_URL_PREFIX to
 # something other than '/'.
-#PUBLIC_URL_PREFIX = "/"
+#PUBLIC_URL_PREFIX = getenv("CHILL_PUBLIC_URL_PREFIX", default="/")
 
 # If setting the ROOT_FOLDER:
-#PUBLIC_URL_PREFIX = "/site"
+#PUBLIC_URL_PREFIX = getenv("CHILL_PUBLIC_URL_PREFIX", default="/site")
 
 # The ROOT_FOLDER is used to send static files from the '/' route.  This will
 # conflict with the default value for PUBLIC_URL_PREFIX. Any file or directory
 # within the ROOT_FOLDER will be accessible from '/'.  The default is not
 # having anything set.
-#ROOT_FOLDER = "root"
+#ROOT_FOLDER = getenv("CHILL_ROOT_FOLDER", default="root")
 
 # The document folder is an optional way of storing content outside of the
 # database.  It is used with the custom filter 'readfile' which can read the
 # file from the document folder into the template.  If it is a Markdown file
 # you can also use another filter to parse the markdown into HTML with the
 # 'markdown' filter. For example:
 # {{ 'llamas-are-cool.md'|readfile|markdown }}
-# DOCUMENT_FOLDER = "documents"
+#DOCUMENT_FOLDER = getenv("CHILL_DOCUMENT_FOLDER", default="documents")
 
 # The media folder is used to send static files that are not related to the
 # 'theme' of a site.  This usually includes images and videos that are better
 # served from the file system instead of the database. The default is not
 # having this set to anything.
-#MEDIA_FOLDER = "media"
+#MEDIA_FOLDER = getenv("CHILL_MEDIA_FOLDER", default="media")
 
 # The media path is where the files in the media folder will be accessible.  In
 # templates you can use the custom variable: 'media_path' which will have this
 # value.
 # {{ media_path }}llama.jpg
 # or:
 # {{ url_for('send_media_file', filename='llama.jpg') }}
-#MEDIA_PATH = "/media/"
+#MEDIA_PATH = getenv("CHILL_MEDIA_PATH", default="/media/")
 
 # When creating a stand-alone static website the files in the MEDIA_FOLDER are
 # only included if they are linked to from a page.  Set this to True if all the
 # files in the media folder should be included in the FREEZER_DESTINATION.
-#MEDIA_FREEZE_ALL = False
+#MEDIA_FREEZE_ALL = getenv("CHILL_MEDIA_FREEZE_ALL", default="False").lower() == "true"
 
 # The theme is where all the front end resources like css, js, graphics and
 # such that make up the theme of a website. The THEME_STATIC_FOLDER is where
 # these files are located and by default nothing is set here.
-#THEME_STATIC_FOLDER = "static"
+#THEME_STATIC_FOLDER = getenv("CHILL_THEME_STATIC_FOLDER", default="static")
 
 # Set a THEME_STATIC_PATH for routing the theme static files with.  It's useful
 # to set a version number within this path to easily do cache-busting.  In your
 # templates you can use the custom variable:
 # {{ theme_static_path }}llama.css
 # or:
 # {{ url_for('send_theme_file', filename='llama.css') }}
 # to get the url to a file in the theme static folder.
-#THEME_STATIC_PATH = "/theme/v0.0.1/"
+
+VERSION = "0"
+PACKAGEJSON = {}
+if isfile('package.json'):
+    with open('package.json') as f:
+        PACKAGEJSON = json.load(f)
+        VERSION = PACKAGEJSON['version']
+elif isfile('VERSION'):
+    with open('VERSION') as f:
+        VERSION = f.read().strip()
+
+THEME_STATIC_PATH = getenv("CHILL_THEME_STATIC_PATH", default="/theme/{VERSION}/").format(**locals())
 
 # Where the jinja2 templates for the site are located.  Will default to the app
 # template_folder if not set.
-THEME_TEMPLATE_FOLDER = "templates"
+THEME_TEMPLATE_FOLDER = getenv("CHILL_THEME_TEMPLATE_FOLDER", default="templates")
 
 # Where all the custom SQL queries and such are located.  Chill uses a few
 # built-in ones and they can be overridden by adding a file with the same name
 # in here. To do much of anything with Chill you will need to add some custom
 # SQL queries and such to load data into your templates.
-#THEME_SQL_FOLDER = "queries"
+#THEME_SQL_FOLDER = getenv("CHILL_THEME_SQL_FOLDER", default="queries")
 
 # Helpful to have this set to True if you want to fix stuff.
-#DEBUG=True
-
-# Caching with Flask-Cache
-CACHE_NO_NULL_WARNING = True
-CACHE_TYPE = "null"
-#CACHE_TYPE = "simple"
-#CACHE_TYPE = "filesystem"
+#DEBUG = getenv("CHILL_DEBUG", default="False").lower() == "true"
 
+# https://pythonhosted.org/Frozen-Flask/#configuration
 # For creating a stand-alone static website that you can upload without
 # requiring an app to run it. This will use Frozen-Flask.
 # The path to the static/frozen website will be put.
-#FREEZER_DESTINATION = "/home/something/path/to/frozen"
+FREEZER_DESTINATION = getenv("CHILL_FREEZER_DESTINATION", default="frozen")
+#FREEZER_BASE_URL = getenv("CHILL_FREEZER_BASE_URL", default="//{HOSTNAME}/").format(**locals())
 """
 
 
 def main():
-    ""
+    """"""
     args = docopt(__doc__, version=__version__)
     # parse args and pass to run, server, etc.
     if args["init"]:
         init()
 
     if args["initdb"]:
         initdb(args["--config"])
 
+    if args["dropdb"]:
+        dropdb(args["--config"])
+
     if args["run"]:
         run(args["--config"], database_readonly=args.get("--readonly", False))
 
-    if args["operate"]:
-        operate(args["--config"])
-
     if args["load"]:
         load(args["--config"], yaml_file=args.get("--yaml", "chill-data.yaml"))
 
     if args["dump"]:
         dump(args["--config"], yaml_file=args.get("--yaml", "chill-data.yaml"))
 
     if args["migrate"]:
@@ -197,82 +207,89 @@
     main()
 
 
 def initdb(config):
     "Initialize Chill database tables only."
 
     app = make_app(config=config)
+    set_sqlite_journal_mode(app)
 
     with app.app_context():
         app.logger.info("initializing database")
-        init_db()
+        db = get_db()
+        with db:
+            init_db()
+
+
+def dropdb(config):
+    "Deletes Chill database tables only."
+
+    app = make_app(config=config)
+    set_sqlite_journal_mode(app)
+
+    with app.app_context():
+        app.logger.info("Removing Chill database tables: Chill, Node, Node_Node, Route, Query, Template.")
+        db = get_db()
+        with db:
+            drop_db()
 
 
 def init():
     "Initialize the current directory with base starting files and database."
 
     if not os.path.exists("site.cfg"):
-        f = open("site.cfg", "w")
-        f.write(SITECFG)
-        f.close()
+        with open("site.cfg", "w") as f:
+            f.write(SITECFG)
 
     try:
         os.mkdir("queries")
     except OSError:
         pass
 
     try:
         os.mkdir("templates")
     except OSError:
         pass
 
     htmlfile = os.path.join("templates", "homepage.html")
     if not os.path.exists(htmlfile):
-        f = open(htmlfile, "w")
-        f.write(
+        with open(htmlfile, "w") as f:
+            f.write(
+                """
+    <!doctype html>
+    <html>
+        <head>
+            <title>Chill</title>
+        </head>
+        <body>
+            <p>{{ homepage_content }}</p>
+        </body>
+    </html>
             """
-<!doctype html>
-<html>
-    <head>
-        <title>Chill</title>
-    </head>
-    <body>
-        <p>{{ homepage_content }}</p>
-    </body>
-</html>
-        """
-        )
-        f.close()
+            )
 
     app = make_app(config="site.cfg", DEBUG=True)
+    set_sqlite_journal_mode(app)
 
     with app.app_context():
         app.logger.info("initializing database")
-        init_db()
-
-        homepage = insert_node(name="homepage", value=None)
-        insert_route(path="/", node_id=homepage)
-        insert_query(name="select_link_node_from_node.sql", node_id=homepage)
-
-        add_template_for_node("homepage.html", homepage)
-
-        homepage_content = insert_node(
-            name="homepage_content", value="Cascading, Highly Irrelevant, Lost Llamas"
-        )
-        insert_node_node(node_id=homepage, target_node_id=homepage_content)
-
+        db = get_db()
+        with db:
+            init_db()
+
+            homepage = insert_node(name="homepage", value=None)
+            insert_route(path="/", node_id=homepage)
+            insert_query(name="select_link_node_from_node.sql", node_id=homepage)
 
-def operate(config):
-    "Interface to do simple operations on the database."
-
-    app = make_app(config=config)
+            add_template_for_node("homepage.html", homepage)
 
-    print("Operate Mode")
-    with app.app_context():
-        operate_menu()
+            homepage_content = insert_node(
+                name="homepage_content", value="Cascading, Highly Irrelevant, Lost Llamas"
+            )
+            insert_node_node(node_id=homepage, target_node_id=homepage_content)
 
 
 def load(config, yaml_file):
     "Load a yaml file that has ChillNode objects into the database."
 
     app = make_app(config=config)
 
@@ -293,29 +310,50 @@
     "Migrate the database from a previous version to a new one."
 
     app = make_app(config=config)
 
     with app.app_context():
         migrate1()
 
+
 def set_sqlite_journal_mode(app):
 
-    db_file = app.config.get("CHILL_DATABASE_URI")[len("sqlite:///"):]
+    db_file = app.config.get("CHILL_DATABASE_URI")
     journal_mode = app.config.get("SQLITE_JOURNAL_MODE")
     if not journal_mode or not isinstance(journal_mode, str):
         return
 
-    if not journal_mode.lower() in ("delete", "truncate" , "persist" , "memory" , "wal" , "off"):
+    if not journal_mode.lower() in (
+        "delete",
+        "truncate",
+        "persist",
+        "memory",
+        "wal",
+        "off",
+    ):
         return
 
     if db_file and not db_file.startswith(":"):
         # Need to set Write-Ahead Logging so multiple apps can work with the db
         # concurrently.  https://sqlite.org/wal.html
-        app.logger.info("set journal mode to '{}' on db file: {}".format(journal_mode, db_file))
-        subprocess.run(["sqlite3", db_file, "pragma journal_mode={journal_mode}".format(journal_mode=journal_mode)])
+        app.logger.info(
+            "set journal mode to '{}' on db file: {}".format(journal_mode, db_file)
+        )
+        set_journal_mode_output = subprocess.run(
+            [
+                "sqlite3",
+                db_file,
+                "pragma journal_mode={journal_mode}".format(journal_mode=journal_mode),
+            ],
+            capture_output=True,
+            check=True,
+        )
+        app.logger.info(" ".join(set_journal_mode_output.args))
+        app.logger.info(set_journal_mode_output.stdout.decode())
+
 
 # bin/run
 def run(config, database_readonly=False):
     "Start the web server in the foreground. Don't use for production."
     app = make_app(config=config, database_readonly=database_readonly)
 
     set_sqlite_journal_mode(app)
@@ -337,80 +375,70 @@
 
     set_sqlite_journal_mode(app)
 
     host = app.config.get("HOST", "127.0.0.1")
     port = app.config.get("PORT", 5000)
     app.logger.info("serving on {host}:{port}".format(**locals()))
     http_server = pywsgi.WSGIServer((host, port), app)
+
     def shutdown():
         app.logger.info("Stopping Chill app")
         http_server.stop(timeout=10)
         exit(signal.SIGTERM)
 
     signal_handler(signal.SIGTERM, shutdown)
     signal_handler(signal.SIGINT, shutdown)
     http_server.serve_forever(stop_timeout=10)
 
 
 # bin/freeze
 def freeze(config, urls_file=None):
     """Freeze the application by creating a static version of it."""
     if urls_file:
-        app = make_app(config=config, URLS_FILE=urls_file)
+        app = make_app(config=config, URLS_FILE=urls_file, database_readonly=True)
     else:
-        app = make_app(config=config)
+        app = make_app(config=config, database_readonly=True)
     app.logger.info("freezing app to directory: %s" % app.config["FREEZER_DESTINATION"])
     freezer = Freezer(app)
 
-    # @freezer.register_generator
-    # def index_page():
-    #    for (dirpath, dirnames, filenames) in os.walk(app.config['DATA_PATH'], topdown=True):
-    #        start = len(os.path.commonprefix((app.config['DATA_PATH'], dirpath)))
-    #        relative_path = dirpath[start+1:]
-    #        for dirname in dirnames:
-    #            yield ('page.index_page', {'uri': os.path.join(relative_path, dirname)})
-
-    # @freezer.register_generator
-    # def page_uri():
-    #    # uri_index will be used so just avoid showing a warning
-    #    return [
-    #            ('public.page_uri', {'uri': ''}),
-    #            ]
     @freezer.register_generator
     def uri_index():
         def cleanup_url(url):
             url = url.strip()
             if url.startswith("/"):
                 if url.endswith("/index.html"):
                     return url
                 elif url.endswith("/"):
                     url = url.strip("/")
                     if len(url) == 0:
                         return ("public.index", {})
                     return ("public.uri_index", {"uri": url})
 
+        db = get_db()
+        cur = db.cursor()
         try:
-            result = db.execute(
-                text(fetch_query_string("select_paths_to_freeze.sql"))
+            result = cur.execute(
+                fetch_query_string("select_paths_to_freeze.sql")
             ).fetchall()
-        except (DatabaseError, StatementError) as err:
+        except (sqlite3.Error) as err:
             app.logger.error("DatabaseError: %s", err)
             return []
         urls = [_f for _f in [cleanup_url(x[0]) for x in result] if _f]
 
         urls_file = app.config.get("URLS_FILE", None)
         if urls_file:
             urls_file = (
                 urls_file
                 if urls_file[0] == os.sep
                 else os.path.join(os.getcwd(), urls_file)
             )
-            f = open(urls_file, "r")
-            urls.extend([_f for _f in map(cleanup_url, f.readlines()) if _f])
-            f.close()
+            with open(urls_file, "r") as f:
+                urls.extend([_f for _f in map(cleanup_url, f.readlines()) if _f])
+
+        cur.close()
 
         return urls
 
     @freezer.register_generator
     def send_root_file():
         root_folder = app.config.get("ROOT_FOLDER", None)
         if root_folder and os.path.isdir(root_folder):
```

### Comparing `chill-0.8.1/src/chill/shortcodes.py` & `chill-0.9.0/src/chill/shortcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,117 +44,120 @@
 `context` argument accepts an arbitrary object to pass on to the registered
 handler functions.
 
 Author: Darren Mulholland <dmulholland@outlook.ie>
 License: This work has been placed in the public domain.
 
 """
-from __future__ import print_function
 
-from builtins import bytes
-from builtins import str
-from builtins import object
+
 __version__ = "2.0.1"
 
 
 import re
-import sys
 
 
 # Stores registered shortcode functions indexed by tag.
-tagmap = { 'endtags': [] }
+tagmap = {"endtags": []}
 
 
 def register(tag, end_tag=None):
-    """ Decorator for registering shortcode functions. """
+    """Decorator for registering shortcode functions."""
 
     def register_function(function):
-        tagmap[tag] = {'func': function, 'endtag': end_tag}
+        tagmap[tag] = {"func": function, "endtag": end_tag}
         if end_tag:
-            tagmap['endtags'].append(end_tag)
+            tagmap["endtags"].append(end_tag)
         return function
 
     return register_function
 
 
 def decode(s):
-    """ Decode string escape sequences. """
-    return bytes(s, 'utf-8').decode('unicode_escape')
+    """Decode string escape sequences."""
+    return bytes(s, "utf-8").decode("unicode_escape")
 
 
 class ShortcodeError(Exception):
-    """ Base class for all exceptions raised by the module. """
+    """Base class for all exceptions raised by the module."""
+
     pass
 
 
 class NestingError(ShortcodeError):
-    """ Raised if the parser detects unbalanced tags. """
+    """Raised if the parser detects unbalanced tags."""
+
     pass
 
 
 class InvalidTagError(ShortcodeError):
-    """ Raised if the parser encounters an unknown tag. """
+    """Raised if the parser encounters an unknown tag."""
+
     pass
 
 
 class RenderingError(ShortcodeError):
-    """ Raised if an attempt to call a shortcode function fails. """
+    """Raised if an attempt to call a shortcode function fails."""
+
     pass
 
 
 class Node(object):
 
-    """ Input text is parsed into a tree of Node objects. """
+    """Input text is parsed into a tree of Node objects."""
 
     def __init__(self):
         self.children = []
 
     def render(self, context):
-        return u''.join(child.render(context) for child in self.children)
+        return u"".join(child.render(context) for child in self.children)
 
 
 class TextNode(Node):
 
-    """ Plain text content. """
+    """Plain text content."""
 
     def __init__(self, text):
         self.text = text
 
     def render(self, context):
         return self.text
 
 
 class ShortcodeNode(Node):
 
-    """ An atomic (non-block-scoped) shortcode. """
+    """An atomic (non-block-scoped) shortcode."""
 
-    argregex = re.compile(r"""
+    argregex = re.compile(
+        r"""
         (?:([^\s'"=]+)=)?
         (
             "((?:[^\\"]|\\.)*)"
             |
             '((?:[^\\']|\\.)*)'
         )
         |
         ([^\s'"=]+)=(\S+)
         |
         (\S+)
-    """, re.VERBOSE)
+    """,
+        re.VERBOSE,
+    )
 
     def __init__(self, tag, argstring):
         self.tag = tag
-        self.func = tagmap[tag]['func']
+        self.func = tagmap[tag]["func"]
         self.pargs, self.kwargs = self.parse_args(argstring)
 
     def render(self, context):
         try:
             return str(self.func(context, None, self.pargs, self.kwargs))
         except Exception as e:
             print(e)
-            raise RenderingError('error rendering [%s] tag' % self.tag)
+            raise RenderingError("error rendering [%s] tag" % self.tag)
 
     def parse_args(self, argstring):
         pargs, kwargs = [], {}
         for match in self.argregex.finditer(argstring):
             if match.group(2) or match.group(5):
                 key = match.group(1) or match.group(5)
                 value = match.group(3) or match.group(4) or match.group(6)
@@ -167,97 +170,100 @@
             else:
                 pargs.append(match.group(7))
         return pargs, kwargs
 
 
 class ScopedShortcodeNode(ShortcodeNode):
 
-    """ A block-scoped shortcode. """
+    """A block-scoped shortcode."""
 
     def __init__(self, tag, argstring):
         ShortcodeNode.__init__(self, tag, argstring)
         self.children = []
 
     def render(self, context):
-        content = u''.join(child.render(context) for child in self.children)
+        content = u"".join(child.render(context) for child in self.children)
         try:
             return str(self.func(context, content, self.pargs, self.kwargs))
         except:
-            raise RenderingError('error rendering [%s] tag' % self.tag)
+            raise RenderingError("error rendering [%s] tag" % self.tag)
 
 
 class Parser(object):
 
-    """ Parses text and renders shortcodes.
+    """Parses text and renders shortcodes.
 
     A single Parser instance can parse mulitple input strings.
 
         parser = Parser()
         output = parser.parse(text, context)
 
     The .parse() method accepts an arbitrary context object which it
     passes on to the shortcode handler functions.
 
     """
 
-    def __init__(self, start='[%', end='%]', esc='\\'):
+    def __init__(self, start="[%", end="%]", esc="\\"):
         self.start = start
         self.estart = esc + start
         self.len_start = len(start)
         self.len_end = len(end)
         self.len_esc = len(esc)
-        self.regex = re.compile(r'((?:%s)?%s.*?%s)' % (
-            re.escape(esc),
-            re.escape(start),
-            re.escape(end),
-        ))
+        self.regex = re.compile(
+            r"((?:%s)?%s.*?%s)"
+            % (
+                re.escape(esc),
+                re.escape(start),
+                re.escape(end),
+            )
+        )
 
     def parse(self, text, context=None):
         stack, expecting = [], []
         stack.append(Node())
 
         for token in self.tokenize(text):
             if token.startswith(self.start):
-                content = token[self.len_start:-self.len_end].strip()
+                content = token[self.len_start : -self.len_end].strip()
                 if content:
                     self.parse_token_content(stack, expecting, content)
             elif token.startswith(self.estart):
-                stack[-1].children.append(TextNode(token[self.len_esc:]))
+                stack[-1].children.append(TextNode(token[self.len_esc :]))
             else:
                 stack[-1].children.append(TextNode(token))
 
         if expecting:
-            raise NestingError('expecting [%s]' % expecting[-1])
+            raise NestingError("expecting [%s]" % expecting[-1])
 
         return stack.pop().render(context)
 
     def tokenize(self, text):
         for token in self.regex.split(text):
             if token:
                 yield token
 
     def parse_token_content(self, stack, expecting, content):
         tag = content.split(None, 1)[0]
 
-        if tag in tagmap['endtags']:
+        if tag in tagmap["endtags"]:
             if not expecting:
-                raise NestingError('not expecting [%s]' % tag)
+                raise NestingError("not expecting [%s]" % tag)
             elif tag == expecting[-1]:
                 stack.pop()
                 expecting.pop()
             else:
-                msg = 'expecting [%s], found [%s]'
+                msg = "expecting [%s], found [%s]"
                 raise NestingError(msg % (expecting[-1], tag))
 
         elif tag in tagmap:
-            if tagmap[tag]['endtag']:
-                node = ScopedShortcodeNode(tag, content[len(tag):])
+            if tagmap[tag]["endtag"]:
+                node = ScopedShortcodeNode(tag, content[len(tag) :])
                 stack[-1].children.append(node)
                 stack.append(node)
-                expecting.append(tagmap[tag]['endtag'])
+                expecting.append(tagmap[tag]["endtag"])
             else:
-                node = ShortcodeNode(tag, content[len(tag):])
+                node = ShortcodeNode(tag, content[len(tag) :])
                 stack[-1].children.append(node)
 
         else:
-            msg = '[%s] is not a recognised shortcode tag'
+            msg = "[%s] is not a recognised shortcode tag"
             raise InvalidTagError(msg % tag)
```

### Comparing `chill-0.8.1/src/chill/test_api.py` & `chill-0.9.0/src/chill/test_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 import unittest
 
-from chill.api import (
-        _short_circuit
-        )
+from chill.api import _short_circuit
 
 
 class ApiTestCase(unittest.TestCase):
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-class ShortCircuit(ApiTestCase):
 
+class ShortCircuit(ApiTestCase):
     def test_short_circuit_skip(self):
-        a = 'Johnny'
+        a = "Johnny"
         b = _short_circuit(a)
         assert a == b
 
-        a = ['Johnny', 'Johnny Five']
+        a = ["Johnny", "Johnny Five"]
         b = _short_circuit(a)
         assert a == b
 
-        a = {'id':5}
+        a = {"id": 5}
         b = _short_circuit(a)
         assert a == b
 
-        a = {'id':5,'name':'Johnny'}
+        a = {"id": 5, "name": "Johnny"}
         b = _short_circuit(a)
         assert a == b
 
-        a = [{'id':5},{'id':4}]
+        a = [{"id": 5}, {"id": 4}]
         b = _short_circuit(a)
         assert a == b
 
     def test_short_circuit_list(self):
-        a = ['Johnny']
+        a = ["Johnny"]
         b = _short_circuit(a)
-        assert b == 'Johnny'
+        assert b == "Johnny"
 
-        a = [['Johnny']]
+        a = [["Johnny"]]
         b = _short_circuit(a)
-        assert b == 'Johnny'
+        assert b == "Johnny"
 
-        a = [[{'id':5},{'id':4}]]
+        a = [[{"id": 5}, {"id": 4}]]
         b = _short_circuit(a)
-        assert b == [{'id':5},{'id':4}]
+        assert b == [{"id": 5}, {"id": 4}]
 
     def test_short_circuit_dict(self):
-        a = [{'id':5,'name':'Johnny Five'}]
+        a = [{"id": 5, "name": "Johnny Five"}]
         b = _short_circuit(a)
-        assert b == {'id':5,'name':'Johnny Five'}
+        assert b == {"id": 5, "name": "Johnny Five"}
 
-        a = [{'id':5},{'name':'Johnny Five'}]
+        a = [{"id": 5}, {"name": "Johnny Five"}]
         b = _short_circuit(a)
-        assert b == {'id':5,'name':'Johnny Five'}
+        assert b == {"id": 5, "name": "Johnny Five"}
 
-        a = [{'id':5, 'status':'unknown'},{'name':'Johnny Five'}]
+        a = [{"id": 5, "status": "unknown"}, {"name": "Johnny Five"}]
         b = _short_circuit(a)
         assert a == b
 
-        a = [{'id':5,'name':'Johnny Five'}, {'id':4,'name':'unknown'}]
+        a = [{"id": 5, "name": "Johnny Five"}, {"id": 4, "name": "unknown"}]
         b = _short_circuit(a)
         assert a == b
 
-        a = {'name':'Number Five', 'manufacturer':'NOVA Laboratories'}
+        a = {"name": "Number Five", "manufacturer": "NOVA Laboratories"}
         b = _short_circuit(a)
         assert a == b
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
-
```

### Comparing `chill-0.8.1/src/chill/test_loader.py` & `chill-0.9.0/src/chill/test_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,115 @@
 import unittest
 import tempfile
 import os
 
 from chill.app import multiple_directory_files_loader
 
+
 class LoadSelectSql(unittest.TestCase):
     def setUp(self):
         self.dir_a = tempfile.mkdtemp()
         self.dir_b = tempfile.mkdtemp()
 
     def tearDown(self):
         for tmp_dir in (self.dir_a, self.dir_b):
-            for root, dirs, files in os.walk( tmp_dir, topdown=False ):
+            for root, dirs, files in os.walk(tmp_dir, topdown=False):
                 for name in files:
                     os.remove(os.path.join(root, name))
                 for name in dirs:
                     os.rmdir(os.path.join(root, name))
             os.rmdir(tmp_dir)
 
-
     def write_dict_to_files(self, d, dirname):
         for (k, v) in list(d.items()):
             # mkdir that are in the path (if any)
-            dirs = k.split('/')[:-1]
+            dirs = k.split("/")[:-1]
             if len(dirs) > 0:
                 try:
-                    os.makedirs( os.path.join( dirname, os.path.dirname(k) ) )
+                    os.makedirs(os.path.join(dirname, os.path.dirname(k)))
                 except OSError:
                     pass
-                    #print 'exists ' + os.path.join( dirname, os.path.dirname(k) )
-            with open( os.path.join(dirname, k), 'w') as f:
-                f.write( v )
+                    # print 'exists ' + os.path.join( dirname, os.path.dirname(k) )
+            with open(os.path.join(dirname, k), "w") as f:
+                f.write(v)
 
     def test_one_dir_with_one_file(self):
-        self.write_dict_to_files({
-            'abc': 'a value',
-            }, self.dir_a)
+        self.write_dict_to_files(
+            {
+                "abc": "a value",
+            },
+            self.dir_a,
+        )
 
         a = multiple_directory_files_loader(self.dir_a)
-        assert a.get('abc') == 'a value'
+        assert a.get("abc") == "a value"
 
     def test_two_dir_with_one_file(self):
-        self.write_dict_to_files({
-            'abc': 'a value',
-            }, self.dir_a)
-        self.write_dict_to_files({
-            'abc': 'b value',
-            }, self.dir_b)
+        self.write_dict_to_files(
+            {
+                "abc": "a value",
+            },
+            self.dir_a,
+        )
+        self.write_dict_to_files(
+            {
+                "abc": "b value",
+            },
+            self.dir_b,
+        )
 
         a = multiple_directory_files_loader(self.dir_a, self.dir_b)
-        assert a.get('abc') == 'b value'
+        assert a.get("abc") == "b value"
 
     def test_two_dir_with_more_files(self):
-        self.write_dict_to_files({
-            'abc': 'a value',
-            'a': '1',
-            }, self.dir_a)
-        self.write_dict_to_files({
-            'abc': 'b value',
-            'b': '2',
-            }, self.dir_b)
+        self.write_dict_to_files(
+            {
+                "abc": "a value",
+                "a": "1",
+            },
+            self.dir_a,
+        )
+        self.write_dict_to_files(
+            {
+                "abc": "b value",
+                "b": "2",
+            },
+            self.dir_b,
+        )
 
         a = multiple_directory_files_loader(self.dir_a, self.dir_b)
-        assert a.get('abc') == 'b value'
-        assert a.get('a') == '1'
-        assert a.get('b') == '2'
+        assert a.get("abc") == "b value"
+        assert a.get("a") == "1"
+        assert a.get("b") == "2"
 
     def test_two_dir_with_subfiles(self):
-        self.write_dict_to_files({
-            'abc/dog': 'a value',
-            'a/b/c/dog': '1',
-            'a/blue': '1',
-            'cat': '1',
-            }, self.dir_a)
-        self.write_dict_to_files({
-            'abc/dog': 'b value',
-            'cat': '2',
-            'a/b/c/dog': '2',
-            'a/dog': '2',
-            'a/b/cat': '2',
-            }, self.dir_b)
+        self.write_dict_to_files(
+            {
+                "abc/dog": "a value",
+                "a/b/c/dog": "1",
+                "a/blue": "1",
+                "cat": "1",
+            },
+            self.dir_a,
+        )
+        self.write_dict_to_files(
+            {
+                "abc/dog": "b value",
+                "cat": "2",
+                "a/b/c/dog": "2",
+                "a/dog": "2",
+                "a/b/cat": "2",
+            },
+            self.dir_b,
+        )
 
         a = multiple_directory_files_loader(self.dir_a, self.dir_b)
-        assert a.get('abc/dog') == 'b value'
-        assert a.get('a') == None
-        assert a.get('cat') == '2'
-        assert a.get('a/b/c/dog') == '2'
-        assert a.get('a/b') == None
-        assert a.get('a/b/cat') == '2'
+        assert a.get("abc/dog") == "b value"
+        assert a.get("a") == None
+        assert a.get("cat") == "2"
+        assert a.get("a/b/c/dog") == "2"
+        assert a.get("a/b") == None
+        assert a.get("a/b/cat") == "2"
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `chill-0.8.1/src/chill/tests.py` & `chill-0.9.0/src/chill/tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # -*- coding: utf-8 -*-
 
-from builtins import range, bytes
 import unittest
 import tempfile
 import os
 import json
 import logging
+import sqlite3
 
-from sqlalchemy.exc import OperationalError
-from sqlalchemy.sql import text
 import yaml
 
-from chill.app import make_app, db
+from chill.app import make_app
 from chill.database import (
+    get_db,
+    close_db,
     init_db,
-    rowify,
+    drop_db,
     insert_node,
     insert_node_node,
     select_node,
     delete_node,
     insert_route,
     insert_query,
     fetch_query_string,
     add_template_for_node,
 )
 from chill.yaml_chill_node import load_yaml, dump_yaml, ChillNode
 
 
 class ChillTestCase(unittest.TestCase):
-    database_readonly=False
+    database_readonly = False
+
     def setUp(self):
         self.debug = False
         self.tmp_template_dir = tempfile.mkdtemp()
         self.tmp_db = tempfile.NamedTemporaryFile(delete=False)
         self.app = make_app(
-            CHILL_DATABASE_URI="sqlite:///" + self.tmp_db.name,
+            CHILL_DATABASE_URI=self.tmp_db.name,
+            SQLITE_JOURNAL_MODE="wal",
             THEME_TEMPLATE_FOLDER=self.tmp_template_dir,
             THEME_SQL_FOLDER=self.tmp_template_dir,
             MEDIA_FOLDER=self.tmp_template_dir,
             DOCUMENT_FOLDER=self.tmp_template_dir,
             CACHE_NO_NULL_WARNING=True,
             DEBUG=self.debug,
+            TESTING=True,
             database_readonly=self.database_readonly,
         )
         self.app.logger.setLevel(logging.DEBUG if self.debug else logging.CRITICAL)
 
     def tearDown(self):
         """Get rid of the database and templates after each test."""
         # self.tmp_db.unlink(self.tmp_db.name)
@@ -62,57 +65,266 @@
         os.rmdir(self.tmp_template_dir)
 
 
 class SimpleCheck(ChillTestCase):
     def test_db(self):
         """Check usage of db"""
         with self.app.app_context():
-            with self.app.test_client() as c:
-                init_db()
-
-                db.execute(
-                    text("""insert into Node (name, value) values (:name, :value)"""),
-                    **{"name": "bill", "value": "?"}
-                )
+            with self.app.test_client():
+                db = get_db()
+                with db:
+                    init_db()
+
+                    cur = db.cursor()
+                    cur.execute(
+                        """insert into Node (name, value) values (:name, :value)""",
+                        {"name": "bill", "value": "?"},
+                    )
+                    cur.close()
 
                 # rv = c.get('/bill', follow_redirects=True)
                 # assert '?' in rv.data
 
 
 class SimpleCheckReadonly(ChillTestCase):
-    database_readonly=True
     def test_db_is_readonly(self):
         """Check usage of db"""
         with self.app.app_context():
+            with self.app.test_client():
+                db = get_db()
+                with db:
+                    init_db()
+
+                # Get a new db connection that is readonly
+                close_db()
+                self.app.config["database_readonly"] = True
+                db_ro = get_db()
+                with db_ro:
+                    with self.assertRaises(sqlite3.OperationalError) as err:
+                        cur = db_ro.cursor()
+                        cur.execute(
+                            """insert into Node (name, value) values (:name, :value)""",
+                            {"name": "bill", "value": "?"},
+                        )
+                        cur.close()
+                    self.assertRegex(
+                        str(err.exception), "attempt to write a readonly database"
+                    )
+
+    def test_mutable_methods_when_is_readonly(self):
+        """Check post, put, patch, and delete methods when db is readonly"""
+        with open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w") as f:
+            f.write(
+                """
+              insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "mutate_llama.sql"), "w") as f:
+            f.write(
+                """
+                --- Fake mutate statement. This query shouldn't be called.
+                  Delete from Llama where llama_name = :llama_name;
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
+
+        with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                with self.assertRaises(OperationalError) as err:
-                    db.execute(
-                        text("""insert into Node (name, value) values (:name, :value)"""),
-                        **{"name": "bill", "value": "?"}
+                    cur = db.cursor()
+                    cur.execute(
+                        """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
                     )
-                self.assertRegex(str(err.exception), 'attempt to write a readonly database')
+                    cur.close()
 
+                    llamas_id = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/", node_id=llamas_id, weight=1, method="POST"
+                    )
+                    insert_query(name="insert_llama.sql", node_id=llamas_id)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=llamas_id,
+                        weight=1,
+                        method="PUT",
+                    )
+                    insert_query(name="mutate_llama.sql", node_id=llamas_id)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=llamas_id,
+                        weight=1,
+                        method="PATCH",
+                    )
+                    insert_query(name="mutate_llama.sql", node_id=llamas_id)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=llamas_id,
+                        weight=1,
+                        method="DELETE",
+                    )
+
+                # Insert first llama when db is not readonly
+                llama_1 = {
+                    "llama_name": "Rocky",
+                    "location": "unknown",
+                    "description": "first llama",
+                }
+                rv = c.post("/api/llamas/", data=llama_1)
+                assert 201 == rv.status_code
+
+                # Get a new db connection that is readonly
+                close_db()
+                self.app.config["database_readonly"] = True
+                db_ro = get_db()
+                with db_ro:
+
+                    llama_2 = {
+                        "llama_name": "Nocky",
+                        "location": "unknown",
+                        "description": "second llama",
+                    }
+                    rv = c.post("/api/llamas/", data=llama_2)
+                    assert 400 == rv.status_code
+                    rv = c.put("/api/llamas/name/Nocky/", data=llama_2)
+                    assert 400 == rv.status_code
+                    rv = c.patch("/api/llamas/name/Nocky/", data=llama_2)
+                    assert 400 == rv.status_code
+                    rv = c.delete("/api/llamas/name/Nocky/")
+                    assert 400 == rv.status_code
+
+
+    def test_immutable_methods_when_is_readonly(self):
+        """Check post (which can be immutable) and get methods when db is readonly"""
+        with open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w") as f:
+            f.write(
+                """
+              insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
 
-class Route(ChillTestCase):
-    def test_paths(self):
         with self.app.app_context():
-            init_db()
+            with self.app.test_client() as c:
+                db = get_db()
+                with db:
+                    init_db()
 
-            top_id = insert_node(name="top", value="hello")
-            insert_route(path="/", node_id=top_id)
+                    cur = db.cursor()
+                    cur.execute(
+                        """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
+                    )
+                    cur.close()
 
-            one_id = insert_node(name="one", value="1")
-            insert_route(path="/one/", node_id=one_id)
-            two_id = insert_node(name="two", value="2")
-            insert_route(path="/one/two/", node_id=two_id)
-            three_id = insert_node(name="three", value="3")
-            insert_route(path="/one/two/three/", node_id=three_id)
-            insert_route(path="/one/two/other_three/", node_id=three_id)
+                    api_llamas_id = insert_node(name="api_llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/", node_id=api_llamas_id, weight=1, method="POST"
+                    )
+                    insert_query(name="insert_llama.sql", node_id=api_llamas_id)
+
+                    get_llamas_id = insert_node(name="get_llamas", value=None)
+                    insert_route(
+                        path="/search/llamas/", node_id=get_llamas_id, weight=1, method="GET"
+                    )
+                    insert_query(name="select_llama.sql", node_id=get_llamas_id)
+
+                    post_search_llamas_id = insert_node(name="post_search_llamas", value=None)
+                    insert_route(
+                        path="/search/llamas/", node_id=post_search_llamas_id, weight=1, method="POST"
+                    )
+                    insert_query(name="select_llama.sql", node_id=post_search_llamas_id)
+
+                # Insert first llama when db is not readonly
+                llama_1 = {
+                    "llama_name": "Rocky",
+                    "location": "unknown",
+                    "description": "first llama",
+                }
+                rv = c.post("/api/llamas/", data=llama_1)
+                assert 201 == rv.status_code
+
+                # Get a new db connection that is readonly
+                close_db()
+                self.app.config["database_readonly"] = True
+                get_db()
+
+                llama_2 = {
+                    "llama_name": "Nocky",
+                    "location": "unknown",
+                    "description": "second llama",
+                }
+                rv = c.post("/api/llamas/", data=llama_2)
+                assert 400 == rv.status_code
+                close_db()
+
+                get_db()
+                rv = c.post("/search/llamas/", data={"llama_name": "Rocky"})
+                assert 200 == rv.status_code
+                rv_json = json.loads(rv.data)
+                self.app.logger.debug(rv_json)
+                assert set(llama_1.keys()) == set(rv_json.keys())
+                assert set(llama_1.values()) == set(rv_json.values())
+                close_db()
+
+                get_db()
+                rv = c.get("/search/llamas/?llama_name=Rocky")
+                assert 200 == rv.status_code
+                rv_json = json.loads(rv.data)
+                self.app.logger.debug(rv_json)
+                assert set(llama_1.keys()) == set(rv_json.keys())
+                assert set(llama_1.values()) == set(rv_json.values())
+                close_db()
+
+
+class Route(ChillTestCase):
+    def test_paths(self):
+        with self.app.app_context():
+            db = get_db()
+            with db:
+                init_db()
+                self.app.logger.debug(db.execute("select * from Node;").fetchall())
+                top_id = insert_node(name="top", value="hello")
+                self.app.logger.debug(db.execute("select * from Node;").fetchall())
+                self.app.logger.debug(f"top_id {top_id}")
+
+                insert_route(path="/", node_id=top_id)
+
+                one_id = insert_node(name="one", value="1")
+                insert_route(path="/one/", node_id=one_id)
+                two_id = insert_node(name="two", value="2")
+                insert_route(path="/one/two/", node_id=two_id)
+                three_id = insert_node(name="three", value="3")
+                insert_route(path="/one/two/three/", node_id=three_id)
+                insert_route(path="/one/two/other_three/", node_id=three_id)
 
             with self.app.test_client() as c:
 
                 rv = c.get("/", follow_redirects=True)
                 assert b"hello" == rv.data
                 rv = c.get("/.", follow_redirects=True)
                 assert b"hello" == rv.data
@@ -150,64 +362,68 @@
                 )
                 assert b"3" == rv.data
                 rv = c.get("/one/two/other_three/nothing", follow_redirects=True)
                 assert 404 == rv.status_code
 
     def test_single_rule(self):
         with self.app.app_context():
-            init_db()
-
-            id = insert_node(name="top", value="hello")
-            insert_route(path="/<int:count>/", node_id=id)
+            db = get_db()
+            with db:
+                init_db()
+                id = insert_node(name="top", value="hello")
+                insert_route(path="/<int:count>/", node_id=id)
 
             with self.app.test_client() as c:
 
                 rv = c.get("/", follow_redirects=True)
                 assert 404 == rv.status_code
                 rv = c.get("/1", follow_redirects=True)
                 assert b"hello" == rv.data
                 rv = c.get("/1/", follow_redirects=True)
                 assert b"hello" == rv.data
-                rv = c.get("////1/", follow_redirects=True)
-                assert b"hello" == rv.data
+                # No longer supports this
+                # rv = c.get("////1/", follow_redirects=True)
+                # assert b"hello" == rv.data
                 rv = c.get("/1/index.html", follow_redirects=True)
                 assert b"hello" == rv.data
                 rv = c.get("/1/index.html/not", follow_redirects=True)
                 assert 404 == rv.status_code
 
     def test_multiple_rules(self):
         with self.app.app_context():
-            init_db()
-
-            id = insert_node(name="fruit", value="fruit")
-            insert_route(path="/fruit/<anything>/", node_id=id)
-            id = insert_node(name="vegetables", value="vegetables")
-            insert_route(path="/vegetables/<anything>/", node_id=id)
+            db = get_db()
+            with db:
+                init_db()
+                id = insert_node(name="fruit", value="fruit")
+                insert_route(path="/fruit/<anything>/", node_id=id)
+                id = insert_node(name="vegetables", value="vegetables")
+                insert_route(path="/vegetables/<anything>/", node_id=id)
 
             with self.app.test_client() as c:
 
                 rv = c.get("/fruit", follow_redirects=True)
                 assert 404 == rv.status_code
                 rv = c.get("/fruit/pear/", follow_redirects=True)
                 assert b"fruit" == rv.data
                 rv = c.get("/vegetables", follow_redirects=True)
                 assert 404 == rv.status_code
                 rv = c.get("/vegetables/pear/", follow_redirects=True)
                 assert b"vegetables" == rv.data
 
     def test_weight(self):
         with self.app.app_context():
-            init_db()
-
-            id = insert_node(name="a", value="a")
-            insert_route(path="/<path:anything>/", node_id=id, weight=1)
-            id = insert_node(name="aardvark", value="aardvark")
-            insert_route(path="/animals/<anything>/", node_id=id, weight=1)
-            id = insert_node(name="b", value="b")
-            insert_route(path="/<path:something>/", node_id=id, weight=2)
+            db = get_db()
+            with db:
+                init_db()
+                id = insert_node(name="a", value="a")
+                insert_route(path="/<path:anything>/", node_id=id, weight=1)
+                id = insert_node(name="aardvark", value="aardvark")
+                insert_route(path="/animals/<anything>/", node_id=id, weight=1)
+                id = insert_node(name="b", value="b")
+                insert_route(path="/<path:something>/", node_id=id, weight=2)
 
             with self.app.test_client() as c:
 
                 rv = c.get("/apple", follow_redirects=True)
                 assert b"b" == rv.data
                 rv = c.get("/animals/ape", follow_redirects=True)
                 assert b"aardvark" == rv.data
@@ -219,18 +435,19 @@
                 assert b"b" == rv.data
 
     def test_404_on_mismatch_method(self):
         """
         route that matches, but has no method match
         """
         with self.app.app_context():
-            init_db()
-
-            llama_id = insert_node(name="llama", value="1234")
-            insert_route(path="/llama/", node_id=llama_id)
+            db = get_db()
+            with db:
+                init_db()
+                llama_id = insert_node(name="llama", value="1234")
+                insert_route(path="/llama/", node_id=llama_id)
 
             with self.app.test_client() as c:
 
                 rv = c.get("/llama/", follow_redirects=True)
                 assert b"1234" == rv.data
                 assert 200 == rv.status_code
 
@@ -271,423 +488,513 @@
 
 class SQL(ChillTestCase):
     def test_insert_one_node(self):
         """
         Add a node
         """
         with self.app.app_context():
-            init_db()
-            result = db.execute(
-                text(fetch_query_string("insert_node.sql")), name="a", value="apple"
-            )
-            a = result.lastrowid
+            db = get_db()
+            with db:
+                init_db()
+                cur = db.cursor()
+                result = cur.execute(
+                    fetch_query_string("insert_node.sql"), {"name": "a", "value": "apple"}
+                )
+                a = result.lastrowid
 
-            result = db.execute(
-                text("select * from Node where id = :id;"), id=a
+            result = cur.execute(
+                "select * from Node where id = :id;", {"id": a}
             ).fetchall()
+            cur.close()
+
             assert len(result) == 1
             r = result[0]
             assert a == r["id"]
             assert "a" == r["name"]
             assert "apple" == r["value"]
 
     def test_insert_one_node_with_unicode(self):
         """
         Add a node with a unicode value
         """
         with self.app.app_context():
-            init_db()
-            result = db.execute(
-                text(fetch_query_string("insert_node.sql")), name="a", value=u"Àрpĺè"
-            )
-            a = result.lastrowid
+            db = get_db()
+            with db:
+                init_db()
+                cur = db.cursor()
+                result = cur.execute(
+                    fetch_query_string("insert_node.sql"), {"name": "a", "value": u"Àрpĺè"}
+                )
+                a = result.lastrowid
 
-            result = db.execute(
-                text("select * from Node where id = :id;"), id=a
+            result = cur.execute(
+                "select * from Node where id = :id;", {"id": a}
             ).fetchall()
+            cur.close()
+
             assert len(result) == 1
             r = result[0]
             assert a == r["id"]
             assert "a" == r["name"]
             assert u"Àрpĺè" == r["value"]
 
     def test_link(self):
         """
         Link to any node
         """
         with self.app.app_context():
-            init_db()
-            a_id = insert_node(name="a", value=None)
-            b_id = insert_node(name="b", value=None)
-            c_id = insert_node(name="c", value="c")
-            d_id = insert_node(name="d", value="d")
-
-            # a -> c, b -> c
-            # a -> d
-            insert_node_node(node_id=a_id, target_node_id=c_id)
-            insert_node_node(node_id=a_id, target_node_id=d_id)
-            insert_node_node(node_id=b_id, target_node_id=c_id)
-
-            result = db.execute(
-                text(fetch_query_string("select_link_node_from_node.sql")), node_id=a_id
+            db = get_db()
+            with db:
+                init_db()
+                a_id = insert_node(name="a", value=None)
+                b_id = insert_node(name="b", value=None)
+                c_id = insert_node(name="c", value="c")
+                d_id = insert_node(name="d", value="d")
+
+                # a -> c, b -> c
+                # a -> d
+                insert_node_node(node_id=a_id, target_node_id=c_id)
+                insert_node_node(node_id=a_id, target_node_id=d_id)
+                insert_node_node(node_id=b_id, target_node_id=c_id)
+
+            cur = db.cursor()
+            result = cur.execute(
+                fetch_query_string("select_link_node_from_node.sql"), {"node_id": a_id}
             )
             result = [x["node_id"] for x in result]
             assert c_id in result
             assert d_id in result
             assert a_id not in result
 
-            result = db.execute(
-                text(fetch_query_string("select_link_node_from_node.sql")), node_id=b_id
+            result = cur.execute(
+                fetch_query_string("select_link_node_from_node.sql"), {"node_id": b_id}
             )
             result = [x["node_id"] for x in result]
             assert c_id in result
             assert d_id not in result
             assert a_id not in result
+            cur.close()
 
     def test_value(self):
-        """
-        """
+        """ """
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
+                    a_id = insert_node(name="a", value=None)
+                    insert_route(path="/", node_id=a_id)
 
-                a_id = insert_node(name="a", value=None)
-                insert_route(path="/", node_id=a_id)
-
-                content = insert_node(name="content", value="apple")
-                insert_node_node(node_id=a_id, target_node_id=content)
+                    content = insert_node(name="content", value="apple")
+                    insert_node_node(node_id=a_id, target_node_id=content)
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
                 # self.app.logger.debug('test: %s', rv.data)
                 assert b"apple" in rv.data
 
     def test_unicode_value(self):
-        """
-        """
+        """ """
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                a_id = insert_node(name="a", value=None)
-                insert_route(path="/", node_id=a_id)
+                db = get_db()
+                with db:
+                    init_db()
+                    a_id = insert_node(name="a", value=None)
+                    insert_route(path="/", node_id=a_id)
 
-                content = insert_node(name="content", value=u"Àрpĺè")
-                insert_node_node(node_id=a_id, target_node_id=content)
+                    content = insert_node(name="content", value=u"Àрpĺè")
+                    insert_node_node(node_id=a_id, target_node_id=content)
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
                 # assert '\u00c0\u0440p\u013a\u00e8' in bytes(rv.data, 'utf-8').decode('utf-8')
                 assert bytes(b"\u00c0\u0440p\u013a\u00e8") in rv.data
 
     def test_noderequest(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "select_pagenames.sql"), "w")
-        f.write(
-            """
-          select 'yup' as test where :pagename in ('apple', 'pear', 'grapes');
-          """
-        )
-        f.close()
+        """ """
+        with open(
+            os.path.join(self.tmp_template_dir, "select_pagenames.sql"), "w"
+        ) as f:
+            f.write(
+                """
+              select 'yup' as test where :pagename in ('apple', 'pear', 'grapes');
+              """
+            )
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                page = insert_node(name="page", value=None)
-                insert_route(path="/page/<pagename>/", node_id=page)
-
-                pagenames = insert_node(name="pagenames", value=None)
-                insert_node_node(node_id=page, target_node_id=pagenames)
-                insert_query(name="select_pagenames.sql", node_id=pagenames)
+                db = get_db()
+                with db:
+                    init_db()
+                    page = insert_node(name="page", value=None)
+                    insert_route(path="/page/<pagename>/", node_id=page)
+
+                    pagenames = insert_node(name="pagenames", value=None)
+                    insert_node_node(node_id=page, target_node_id=pagenames)
+                    insert_query(name="select_pagenames.sql", node_id=pagenames)
 
                 rv = c.get("/page/cucumber/", follow_redirects=True)
                 assert 200 == rv.status_code
                 # self.app.logger.debug('test: %s', rv.data)
                 assert b"yup" not in rv.data
 
                 rv = c.get("/page/pear/", follow_redirects=True)
                 assert 200 == rv.status_code
                 # self.app.logger.debug('test: %s', rv.data)
                 assert b"yup" in rv.data
 
     def test_noderequest_args(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select :llama as llama;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select :llama as llama;
+              """
+            )
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                page = insert_node(name="page", value=None)
-                insert_route(path="/page/", node_id=page)
-
-                llama = insert_node(name="llama", value=None)
-                insert_node_node(node_id=page, target_node_id=llama)
-                insert_query(name="select_llama.sql", node_id=llama)
+                db = get_db()
+                with db:
+                    init_db()
+                    page = insert_node(name="page", value=None)
+                    insert_route(path="/page/", node_id=page)
+
+                    llama = insert_node(name="llama", value=None)
+                    insert_node_node(node_id=page, target_node_id=llama)
+                    insert_query(name="select_llama.sql", node_id=llama)
 
                 rv = c.get("/page/?llama=chuck", follow_redirects=True)
                 assert 200 == rv.status_code
                 # self.app.logger.debug('test: %s', rv.data)
                 assert b"chuck" in rv.data
 
                 rv = c.get("/page/?nollama=chuck", follow_redirects=True)
                 assert 200 == rv.status_code
                 # self.app.logger.debug('test: %s', rv.data)
                 assert b"chuck" not in rv.data
 
     def test_noderequest_cookies(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select :llama as llama;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select :llama as llama;
+              """
+            )
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                page = insert_node(name="page", value=None)
-                insert_route(path="/page/", node_id=page)
-
-                llama = insert_node(name="llama", value=None)
-                insert_node_node(node_id=page, target_node_id=llama)
-                insert_query(name="select_llama.sql", node_id=llama)
+                db = get_db()
+                with db:
+                    init_db()
+                    page = insert_node(name="page", value=None)
+                    insert_route(path="/page/", node_id=page)
+
+                    llama = insert_node(name="llama", value=None)
+                    insert_node_node(node_id=page, target_node_id=llama)
+                    insert_query(name="select_llama.sql", node_id=llama)
 
                 c.set_cookie("localhost", "llama", "chuck")
 
                 rv = c.get("/page/", follow_redirects=True)
                 assert 200 == rv.status_code
                 # self.app.logger.debug('test: %s', rv.data)
                 assert b"chuck" in rv.data
 
     def test_template(self):
         with self.app.app_context():
-            init_db()
-
-            a = insert_node(name="a", value=None)
-            add_template_for_node("template_a.html", a)
-            aa = insert_node(name="aa", value=None)
-            add_template_for_node("template_a.html", aa)
-            b = insert_node(name="b", value=None)
-            add_template_for_node("template_b.html", b)
-            c = insert_node(name="c", value=None)
-            add_template_for_node("template_c.html", c)
-
-            result = db.execute(
-                text(fetch_query_string("select_template_from_node.sql")), node_id=a
+            db = get_db()
+            with db:
+                init_db()
+                a = insert_node(name="a", value=None)
+                add_template_for_node("template_a.html", a)
+                aa = insert_node(name="aa", value=None)
+                add_template_for_node("template_a.html", aa)
+                b = insert_node(name="b", value=None)
+                add_template_for_node("template_b.html", b)
+                c = insert_node(name="c", value=None)
+                add_template_for_node("template_c.html", c)
+
+            cur = db.cursor()
+            result = cur.execute(
+                fetch_query_string("select_template_from_node.sql"), {"node_id": a}
             )
             result = [x["name"] for x in result]
             assert len(result) == 1
             assert result[0] == "template_a.html"
 
             # another node that uses the same template
-            result = db.execute(
-                text(fetch_query_string("select_template_from_node.sql")), node_id=aa
+            result = cur.execute(
+                fetch_query_string("select_template_from_node.sql"), {"node_id": aa}
             )
             result = [x["name"] for x in result]
             assert len(result) == 1
             assert result[0] == "template_a.html"
 
-            # can overwrite what node is tied to what template
-            add_template_for_node("template_over_a.html", a)
+            with db:
+                # can overwrite what node is tied to what template
+                add_template_for_node("template_over_a.html", a)
 
-            result = db.execute(
-                text(fetch_query_string("select_template_from_node.sql")), node_id=a
+            result = cur.execute(
+                fetch_query_string("select_template_from_node.sql"), {"node_id": a}
             )
             result = [x["name"] for x in result]
             assert len(result) == 1
             assert result[0] == "template_over_a.html"
 
             # this one still uses the other template
-            result = db.execute(
-                text(fetch_query_string("select_template_from_node.sql")), node_id=aa
+            result = cur.execute(
+                fetch_query_string("select_template_from_node.sql"), {"node_id": aa}
             )
             result = [x["name"] for x in result]
             assert len(result) == 1
             assert result[0] == "template_a.html"
 
+            cur.close()
+
     def test_delete_one_node(self):
         """
         Delete a node
         """
         with self.app.app_context():
-            init_db()
-            result = db.execute(
-                text(fetch_query_string("insert_node.sql")), name="a", value="apple"
-            )
-            a = result.lastrowid
+            db = get_db()
+            with db:
+                init_db()
+                cur = db.cursor()
+                result = cur.execute(
+                    fetch_query_string("insert_node.sql"), {"name": "a", "value": "apple"}
+                )
+                a = result.lastrowid
 
-            result = db.execute(
-                text(fetch_query_string("select_node_from_id.sql")), node_id=a
+            result = cur.execute(
+                fetch_query_string("select_node_from_id.sql"), {"node_id": a}
             ).fetchall()
             assert len(result) == 1
             r = result[0]
             assert a == r["node_id"]
             assert "a" == r["name"]
             assert "apple" == r["value"]
 
-            # now delete
-            delete_node(node_id=a)
+            with db:
+                # now delete
+                delete_node(node_id=a)
 
-            result = db.execute(
-                text(fetch_query_string("select_node_from_id.sql")), node_id=a
+            result = cur.execute(
+                fetch_query_string("select_node_from_id.sql"), {"node_id": a}
             ).fetchall()
             assert len(result) == 0
+            cur.close()
 
     def test_delete_node_with_link(self):
         """
         Delete a node also will delete from link
         """
         with self.app.app_context():
-            init_db()
-            a_id = insert_node(name="a", value=None)
-            b_id = insert_node(name="b", value=None)
-            c_id = insert_node(name="c", value="c")
-            d_id = insert_node(name="d", value="d")
-
-            # a -> c, b -> c
-            # a -> d
-            insert_node_node(node_id=a_id, target_node_id=c_id)
-            insert_node_node(node_id=a_id, target_node_id=d_id)
-            insert_node_node(node_id=b_id, target_node_id=c_id)
-
-            result = db.execute(
-                text(fetch_query_string("select_link_node_from_node.sql")), node_id=a_id
+            db = get_db()
+            with db:
+                init_db()
+                a_id = insert_node(name="a", value=None)
+                b_id = insert_node(name="b", value=None)
+                c_id = insert_node(name="c", value="c")
+                d_id = insert_node(name="d", value="d")
+
+                # a -> c, b -> c
+                # a -> d
+                insert_node_node(node_id=a_id, target_node_id=c_id)
+                insert_node_node(node_id=a_id, target_node_id=d_id)
+                insert_node_node(node_id=b_id, target_node_id=c_id)
+
+            cur = db.cursor()
+            result = cur.execute(
+                fetch_query_string("select_link_node_from_node.sql"), {"node_id": a_id}
             )
             result = [x["node_id"] for x in result]
             assert c_id in result
             assert d_id in result
             assert a_id not in result
 
-            result = db.execute(
-                text(fetch_query_string("select_link_node_from_node.sql")), node_id=b_id
+            result = cur.execute(
+                fetch_query_string("select_link_node_from_node.sql"), {"node_id": b_id}
             )
             result = [x["node_id"] for x in result]
             assert c_id in result
             assert d_id not in result
             assert a_id not in result
 
-            # now delete (should use the 'on delete cascade' sql bit)
-            db.execute(text(fetch_query_string("delete_node_for_id.sql")), node_id=a_id)
+            with db:
+                # now delete (should use the 'on delete cascade' sql bit)
+                cur.execute(fetch_query_string("delete_node_for_id.sql"), {"node_id": a_id})
 
-            result = db.execute(
-                text(fetch_query_string("select_node_from_id.sql")), node_id=a_id
+            result = cur.execute(
+                fetch_query_string("select_node_from_id.sql"), {"node_id": a_id}
             ).fetchall()
             assert len(result) == 0
 
-            result = db.execute(
-                text(fetch_query_string("select_link_node_from_node.sql")), node_id=a_id
+            result = cur.execute(
+                fetch_query_string("select_link_node_from_node.sql"), {"node_id": a_id}
             ).fetchall()
             assert len(result) == 0
 
-            result = db.execute(
-                text(fetch_query_string("select_node_node_from_node_id.sql")),
-                node_id=a_id,
+            result = cur.execute(
+                fetch_query_string("select_node_node_from_node_id.sql"),
+                {"node_id": a_id},
             ).fetchall()
 
             assert len(result) == 0
+            cur.close()
 
     def test_select_node(self):
         with self.app.app_context():
-            init_db()
-            simple_id = insert_node(name="simple", value="test")
+            db = get_db()
+            with db:
+                init_db()
+                simple_id = insert_node(name="simple", value="test")
             result = select_node(node_id=simple_id)[0]
             assert set(result.keys()) == set(["name", "value", "node_id"])
             assert result["value"] == "test"
             assert result["name"] == "simple"
             assert result["node_id"] == simple_id
 
+    def test_drop_chill_tables(self):
+        with self.app.app_context():
+            db = get_db()
+            with db:
+                init_db()
+                simple_id = insert_node(name="simple", value="test")
+                result = select_node(node_id=simple_id)[0]
+
+                cur = db.cursor()
+                cur.execute("""
+                    create table Test (
+                        id integer primary key,
+                        favorite_number integer not null,
+                        age integer not null
+                        );
+                    """)
+                cur.execute(
+                    """
+                    insert into Test (
+                        favorite_number,
+                        age
+                        ) values (
+                        :favorite_number,
+                        :age
+                        );
+                    """, {"favorite_number": 5, "age": 37}
+                )
+            result_test_table = cur.execute(
+                """
+                select * from Test where favorite_number = :favorite_number;
+                """, {"favorite_number": 5}
+            ).fetchall()
+            self.app.logger.debug(len(result_test_table))
+            r = result_test_table[0]
+            assert 37 == r["age"]
+
+            assert set(result.keys()) == set(["name", "value", "node_id"])
+            assert result["value"] == "test"
+            assert result["name"] == "simple"
+            assert result["node_id"] == simple_id
+
+            with db:
+                drop_db()
+            result_test_table = cur.execute(
+                """
+                select * from Test where favorite_number = :favorite_number;
+                """, {"favorite_number": 5}
+            ).fetchall()
+            r = result_test_table[0]
+            assert 37 == r["age"]
+
+            with self.assertRaises(sqlite3.OperationalError) as err:
+                # Chill database tables should be dropped, so this would return
+                # an error.
+                result = select_node(node_id=simple_id)[0]
+            self.app.logger.debug(err.exception)
+            self.assertRegex(
+                str(err.exception), "no such table: Node"
+            )
+
 
 class Query(ChillTestCase):
     def test_empty(self):
-        """
-        """
+        """ """
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                # Not setting a value for a node
-                four_id = insert_node(name="empty", value=None)
-                insert_route(path="/empty/", node_id=four_id)
+                    # Not setting a value for a node
+                    four_id = insert_node(name="empty", value=None)
+                    insert_route(path="/empty/", node_id=four_id)
 
                 # When no value is set and no Query or Template is set
                 rv = c.get("/empty", follow_redirects=True)
                 assert 404 == rv.status_code
 
     def test_simple(self):
-        """
-        """
+        """ """
 
-        f = open(os.path.join(self.tmp_template_dir, "simple.sql"), "w")
-        f.write(
-            """
-          select 'yup' as a, 'pretty' as b, 'darn' as c, 'simple' as d;
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "simple.sql"), "w") as f:
+            f.write(
+                """
+              select 'yup' as a, 'pretty' as b, 'darn' as c, 'simple' as d;
+              """
+            )
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                simple_id = insert_node(name="simple", value=None)
-                insert_query(name="simple.sql", node_id=simple_id)
+                    simple_id = insert_node(name="simple", value=None)
+                    insert_query(name="simple.sql", node_id=simple_id)
 
-                insert_route(path="/simple/", node_id=simple_id)
+                    insert_route(path="/simple/", node_id=simple_id)
 
                 rv = c.get("/simple", follow_redirects=True)
                 assert 200 == rv.status_code
                 simple_json = json.loads(rv.data)
                 assert "yup" == simple_json["a"]
 
     def test_rules(self):
-        f = open(os.path.join(self.tmp_template_dir, "insert_promoattr.sql"), "w")
-        f.write(
-            """
-          insert into PromoAttr (node_id, title, description) values (:node_id, :title, :description);
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_promoattr.sql"), "w")
-        f.write(
-            """
-          select * from PromoAttr where node_id = :node_id;
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_promos.sql"), "w")
-        f.write(
-            """
-          select id as node_id, * from Node where name = 'promo' order by id limit 2 offset 13;
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_mainmenu.sql"), "w")
-        f.write(
-            """
-          select name as link from Node where name like 'page_' order by link;
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_pageattr.sql"), "w")
-        f.write(
-            """
-          select 'example title' as title, 'a description of the page' as description;
-          """
-        )
-        f.close()
+        with open(
+            os.path.join(self.tmp_template_dir, "insert_promoattr.sql"), "w"
+        ) as f:
+            f.write(
+                """
+              insert into PromoAttr (node_id, title, description) values (:node_id, :title, :description);
+              """
+            )
+        with open(
+            os.path.join(self.tmp_template_dir, "select_promoattr.sql"), "w"
+        ) as f:
+            f.write(
+                """
+              select * from PromoAttr where node_id = :node_id;
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_promos.sql"), "w") as f:
+            f.write(
+                """
+              select id as node_id, * from Node where name = 'promo' order by id limit 2 offset 13;
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_mainmenu.sql"), "w") as f:
+            f.write(
+                """
+              select name as link from Node where name like 'page_' order by link;
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_pageattr.sql"), "w") as f:
+            f.write(
+                """
+              select 'example title' as title, 'a description of the page' as description;
+              """
+            )
 
         expected = {
             "mainmenu": [{"link": "page1"}, {"link": "page2"}, {"link": "page3"}],
             "pageattr": {
                 "description": "a description of the page",
                 "title": "example title",
             },
@@ -706,372 +1013,419 @@
                         "title": "promo 14",
                     }
                 },
             ],
         }
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                db.execute(
-                    text(
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table PromoAttr (
-                  node_id integer,
-                  abc integer,
-                  title varchar(255),
-                  description text
-                  );
-                """
+                    create table PromoAttr (
+                      node_id integer,
+                      abc integer,
+                      title varchar(255),
+                      description text
+                      );
+                    """
                     )
-                )
 
-                page_id = insert_node(name="page1", value=None)
-                insert_route(path="/page1/", node_id=page_id)
+                    page_id = insert_node(name="page1", value=None)
+                    insert_route(path="/page1/", node_id=page_id)
 
-                pageattr_id = insert_node(name="pageattr", value=None)
-                insert_node_node(node_id=page_id, target_node_id=pageattr_id)
-                insert_query(name="select_pageattr.sql", node_id=pageattr_id)
-
-                mainmenu_id = insert_node(name="mainmenu", value=None)
-                insert_node_node(node_id=page_id, target_node_id=mainmenu_id)
-                insert_query(name="select_mainmenu.sql", node_id=mainmenu_id)
-                # Add some other pages that will be shown in menu as just links
-                insert_node(name="page2", value=None)
-                insert_node(name="page3", value=None)
-
-                promos_id = insert_node(name="promos", value=None)
-                insert_node_node(node_id=page_id, target_node_id=promos_id)
-                insert_query(name="select_promos.sql", node_id=promos_id)
-
-                for a in range(0, 100):
-                    a_id = insert_node(name="promo", value=None)
-                    db.execute(
-                        text(fetch_query_string("insert_promoattr.sql")),
-                        **{
-                            "node_id": a_id,
-                            "title": "promo %i" % a,
-                            "description": "a" * a,
-                        }
-                    )
-                    # wire the promo to it's attr
-                    insert_query(name="select_promoattr.sql", node_id=a_id)
+                    pageattr_id = insert_node(name="pageattr", value=None)
+                    insert_node_node(node_id=page_id, target_node_id=pageattr_id)
+                    insert_query(name="select_pageattr.sql", node_id=pageattr_id)
+
+                    mainmenu_id = insert_node(name="mainmenu", value=None)
+                    insert_node_node(node_id=page_id, target_node_id=mainmenu_id)
+                    insert_query(name="select_mainmenu.sql", node_id=mainmenu_id)
+                    # Add some other pages that will be shown in menu as just links
+                    insert_node(name="page2", value=None)
+                    insert_node(name="page3", value=None)
+
+                    promos_id = insert_node(name="promos", value=None)
+                    insert_node_node(node_id=page_id, target_node_id=promos_id)
+                    insert_query(name="select_promos.sql", node_id=promos_id)
+
+                    for a in range(0, 100):
+                        a_id = insert_node(name="promo", value=None)
+                        cur.execute(
+                            fetch_query_string("insert_promoattr.sql"),
+                            {
+                                "node_id": a_id,
+                                "title": "promo %i" % a,
+                                "description": "a" * a,
+                            },
+                        )
+                        # wire the promo to it's attr
+                        insert_query(name="select_promoattr.sql", node_id=a_id)
+                    cur.close()
+
+                # Get a new db connection that is readonly
+                # self.app.config["database_readonly"] = True
+                # db_ro = get_db(self.app.config)
 
                 rv = c.get("/page1", follow_redirects=True)
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
                 assert 200 == rv.status_code
                 rv_json = json.loads(rv.data)
                 assert set(expected.keys()) == set(rv_json.keys())
                 assert set(expected["pageattr"].keys()) == set(
                     rv_json["pageattr"].keys()
                 )
 
 
 class Template(ChillTestCase):
     def test_some_template(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "base.html"), "w")
-        f.write(
-            """
-          <!doctype html>
-          <html><head><title>test</title></head>
-          <body>
-          <div>{% block content %}{% endblock %}</div>
-          </body>
-          </html>
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "base.html"), "w") as f:
+            f.write(
+                """
+              <!doctype html>
+              <html><head><title>test</title></head>
+              <body>
+              <div>{% block content %}{% endblock %}</div>
+              </body>
+              </html>
+              """
+            )
 
-        f = open(os.path.join(self.tmp_template_dir, "template_a.html"), "w")
-        f.write(
-            """
-          {% extends "base.html" %}
-          {% block content %}
-          <h1>template_a</h1>
-          {{ value }}
-          {% endblock %}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "template_a.html"), "w") as f:
+            f.write(
+                """
+              {% extends "base.html" %}
+              {% block content %}
+              <h1>template_a</h1>
+              {{ value }}
+              {% endblock %}
+              """
+            )
 
-        f = open(os.path.join(self.tmp_template_dir, "template_b.html"), "w")
-        f.write(
-            """
-          {% extends "base.html" %}
-          {% block content %}
-          <h1>template_b</h1>
-          {{ value }}
-          {% endblock %}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "template_b.html"), "w") as f:
+            f.write(
+                """
+              {% extends "base.html" %}
+              {% block content %}
+              <h1>template_b</h1>
+              {{ value }}
+              {% endblock %}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                test_id = insert_node(name="test one", value="testing one")
-                insert_route(path="/test/1/", node_id=test_id)
-                add_template_for_node("template_a.html", test_id)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    test_id = insert_node(name="test one", value="testing one")
+                    insert_route(path="/test/1/", node_id=test_id)
+                    add_template_for_node("template_a.html", test_id)
 
                 rv = c.get("/test/1", follow_redirects=True)
                 assert b"testing one" in rv.data
 
-                a_id = insert_node(name="a", value="apple")
-                insert_route(path="/fruit/a/", node_id=a_id)
-                add_template_for_node("template_a.html", a_id)
+                with db:
+                    a_id = insert_node(name="a", value="apple")
+                    insert_route(path="/fruit/a/", node_id=a_id)
+                    add_template_for_node("template_a.html", a_id)
 
                 rv = c.get("/fruit/a", follow_redirects=True)
                 assert b"apple" in rv.data
                 assert b"template_a" in rv.data
 
-                b_id = insert_node(name="b", value="banana")
-                add_template_for_node("template_b.html", b_id)
-                o_id = insert_node(name="orange", value="orange")
-                add_template_for_node("template_b.html", o_id)
+                with db:
+                    b_id = insert_node(name="b", value="banana")
+                    add_template_for_node("template_b.html", b_id)
+                    o_id = insert_node(name="orange", value="orange")
+                    add_template_for_node("template_b.html", o_id)
 
-                eggplant_id = insert_node(name="eggplant", value="eggplant")
-                add_template_for_node("template_b.html", eggplant_id)
+                    eggplant_id = insert_node(name="eggplant", value="eggplant")
+                    add_template_for_node("template_b.html", eggplant_id)
 
-                # overwrite ( fruit/a use to be set to template_a.html )
-                add_template_for_node("template_b.html", a_id)
+                    # overwrite ( fruit/a use to be set to template_a.html )
+                    add_template_for_node("template_b.html", a_id)
 
                 rv = c.get("/fruit/a", follow_redirects=True)
                 assert b"apple" in rv.data
                 assert b"template_b" in rv.data
 
     def test_some_unicode_as_value_in_template(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "template_unicode.html"), "w")
-        f.write(
-            """
-          <h1>template_unicode</h1>
-          {{ isit|safe }}
-          """
-        )
-        f.close()
+        """ """
+        with open(
+            os.path.join(self.tmp_template_dir, "template_unicode.html"), "w"
+        ) as f:
+            f.write(
+                """
+              <h1>template_unicode</h1>
+              {{ isit|safe }}
+              """
+            )
 
-        f = open(os.path.join(self.tmp_template_dir, "isit.html"), "w")
-        f.write(
-            """
-            <div>template with a unicode {{ value }}</div>
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "isit.html"), "w") as f:
+            f.write(
+                """
+                <div>template with a unicode {{ value }}</div>
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                test_id = insert_node(name="page", value=None)
-                insert_route(path="/test/1/", node_id=test_id)
-                add_template_for_node("template_unicode.html", test_id)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    test_id = insert_node(name="page", value=None)
+                    insert_route(path="/test/1/", node_id=test_id)
+                    add_template_for_node("template_unicode.html", test_id)
 
-                isit = insert_node(name="isit", value=u"Àрpĺè")
-                add_template_for_node("isit.html", isit)
+                    isit = insert_node(name="isit", value=u"Àрpĺè")
+                    add_template_for_node("isit.html", isit)
 
-                insert_node_node(node_id=test_id, target_node_id=isit)
+                    insert_node_node(node_id=test_id, target_node_id=isit)
 
                 rv = c.get("/test/1/", follow_redirects=True)
                 assert u"Àрpĺè" in rv.data.decode("utf-8")
 
     def test_dict(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "llama.html"), "w")
-        f.write(
-            """
-          <!doctype html>
-          <html><head><title>llama</title></head>
-          <body>
-          <h1>template for llama_name</h1>
-          {{ llama_name }}
-          </body>
-          </html>
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select :llama_name as llama_name;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "llama.html"), "w") as f:
+            f.write(
+                """
+              <!doctype html>
+              <html><head><title>llama</title></head>
+              <body>
+              <h1>template for llama_name</h1>
+              {{ llama_name }}
+              </body>
+              </html>
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select :llama_name as llama_name;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                a = insert_node(name="a", value=None)
-                insert_route(path="/a/<llama_name>/", node_id=a)
-                insert_query(name="select_llama.sql", node_id=a)
-                add_template_for_node("llama.html", a)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    a = insert_node(name="a", value=None)
+                    insert_route(path="/a/<llama_name>/", node_id=a)
+                    insert_query(name="select_llama.sql", node_id=a)
+                    add_template_for_node("llama.html", a)
 
                 rv = c.get("/a/chuck/", follow_redirects=True)
                 assert b"chuck" in rv.data
                 rv = c.get("/a/chase/", follow_redirects=True)
                 assert b"chase" in rv.data
 
     def test_chill_now(self):
         """
         Check that the chill_now timestamp is available for templates to use
         """
-        f = open(os.path.join(self.tmp_template_dir, "chill_now.html"), "w")
-        f.write(
-            """
-          {% if chill_now %}timestamp: {{ chill_now }}{% endif %}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "chill_now.html"), "w") as f:
+            f.write(
+                """
+              {% if chill_now %}timestamp: {{ chill_now }}{% endif %}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                a = insert_node(name="a", value=None)
-                insert_route(path="/a/", node_id=a)
-                add_template_for_node("chill_now.html", a)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    a = insert_node(name="a", value=None)
+                    insert_route(path="/a/", node_id=a)
+                    add_template_for_node("chill_now.html", a)
 
                 rv = c.get("/a/", follow_redirects=True)
                 # self.app.logger.debug(rv.data)
                 assert b"timestamp" in rv.data
 
 
 class Filters(ChillTestCase):
     def test_datetime_filter(self):
         """
         The custom 'datetime' jinja2 filter converts a timestamp to a formatted
         date string.
         """
-        f = open(os.path.join(self.tmp_template_dir, "datetime.html"), "w")
-        f.write(
-            """
-          {% set timestamp=1576122368 %}date and time:  {{ timestamp|datetime('y-MM-dd') }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "datetime.html"), "w") as f:
+            f.write(
+                """
+              {% set timestamp=1576122368 %}date and time:  {{ timestamp|datetime('y-MM-dd') }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                a = insert_node(name="a", value=None)
-                insert_route(path="/a/", node_id=a)
-                add_template_for_node("datetime.html", a)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    a = insert_node(name="a", value=None)
+                    insert_route(path="/a/", node_id=a)
+                    add_template_for_node("datetime.html", a)
 
                 rv = c.get("/a/", follow_redirects=True)
                 # self.app.logger.debug(rv.data)
                 assert b"2019-12-12" in rv.data
 
     def test_timedelta_filter(self):
         """
-        The custom 'timedelta' jinja2 filter wraps around the babel format_timedelta.
+        The custom 'timedelta' jinja2 filter wraps around the humanize naturaltime method.
         """
-        f = open(os.path.join(self.tmp_template_dir, "timedelta.html"), "w")
-        f.write(
-            """
-          {% set timesince=847 %}time since:  {{ timesince|timedelta }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "timedelta.html"), "w") as f:
+            f.write(
+                """
+              {% set timesince=847 %}time since:  {{ timesince|timedelta }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                a = insert_node(name="a", value=None)
-                insert_route(path="/a/", node_id=a)
-                add_template_for_node("timedelta.html", a)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    a = insert_node(name="a", value=None)
+                    insert_route(path="/a/", node_id=a)
+                    add_template_for_node("timedelta.html", a)
 
                 rv = c.get("/a/", follow_redirects=True)
                 # self.app.logger.debug(rv.data)
                 assert b"14 minutes" in rv.data
 
 
 class Documents(ChillTestCase):
+    def test_reading_in_a_document_without_setting_document_folder(self):
+        """
+        The custom 'readfile' jinja2 filter shows the file name if the DOCUMENT_FOLDER is not set.
+        """
+        with open(os.path.join(self.tmp_template_dir, "imasimplefile.txt"), "w") as f:
+            f.write(
+                """
+              Hello, this is just a file.
+              """
+            )
+
+        with open(os.path.join(self.tmp_template_dir, "template.html"), "w") as f:
+            f.write(
+                """
+              <h1>template</h1>
+              {{ simplefilename }}
+              <br>
+              {{ simplefilename|readfile }}
+              """
+            )
+
+        # Unset the DOCUMENT_FOLDER
+        self.app.config["DOCUMENT_FOLDER"] = None
+
+        with self.app.app_context():
+            with self.app.test_client() as c:
+                db = get_db()
+                with db:
+                    init_db()
+                    a = insert_node(name="simplefilename", value="imasimplefile.txt")
+                    apage = insert_node(name="apage", value=None)
+                    insert_node_node(node_id=apage, target_node_id=a)
+                    insert_route(path="/a/", node_id=apage)
+                    add_template_for_node("template.html", apage)
+
+                rv = c.get("/a/", follow_redirects=True)
+                assert b"imasimplefile.txt" in rv.data
+
     def test_reading_in_a_document(self):
         """
         The custom 'readfile' jinja2 filter reads the file from the DOCUMENT_FOLDER.
         """
-        f = open(os.path.join(self.tmp_template_dir, "imasimplefile.txt"), "w")
-        f.write(
-            """
-          Hello, this is just a file.
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "imasimplefile.txt"), "w") as f:
+            f.write(
+                """
+              Hello, this is just a file.
+              """
+            )
 
-        f = open(os.path.join(self.tmp_template_dir, "template.html"), "w")
-        f.write(
-            """
-          <h1>template</h1>
-          {{ simplefilename }}
-          <br>
-          {{ simplefilename|readfile }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "template.html"), "w") as f:
+            f.write(
+                """
+              <h1>template</h1>
+              {{ simplefilename }}
+              <br>
+              {{ simplefilename|readfile }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                a = insert_node(name="simplefilename", value="imasimplefile.txt")
-                apage = insert_node(name="apage", value=None)
-                insert_node_node(node_id=apage, target_node_id=a)
-                insert_route(path="/a/", node_id=apage)
-                add_template_for_node("template.html", apage)
+                db = get_db()
+                with db:
+                    init_db()
+                    a = insert_node(name="simplefilename", value="imasimplefile.txt")
+                    apage = insert_node(name="apage", value=None)
+                    insert_node_node(node_id=apage, target_node_id=a)
+                    insert_route(path="/a/", node_id=apage)
+                    add_template_for_node("template.html", apage)
 
                 rv = c.get("/a/", follow_redirects=True)
                 assert b"Hello" in rv.data
 
     def test_reading_in_a_document_with_unicode(self):
         """
         The custom 'readfile' jinja2 filter reads the file with unicode characters from the DOCUMENT_FOLDER.
         """
-        f = open(
+        with open(
             os.path.join(self.tmp_template_dir, "imasimplefilewithunicode.txt"), "w"
-        )
-        f.write(
-            """
-          Hello, this is an Àрpĺè.
-          [chill route /cat/picture/ ]
-          """
-        )
-        f.close()
+        ) as f:
+            f.write(
+                """
+              Hello, this is an Àрpĺè.
+              [chill route /cat/picture/ ]
+              """
+            )
 
-        f = open(os.path.join(self.tmp_template_dir, "template.html"), "w")
-        f.write(
-            """
-          <h1>template</h1>
-          {{ simplefilename }}
-          <br>
-          {{ simplefilename|readfile|safe|shortcodes }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "template.html"), "w") as f:
+            f.write(
+                """
+              <h1>template</h1>
+              {{ simplefilename }}
+              <br>
+              {{ simplefilename|readfile|safe|shortcodes }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                catimg = insert_node(
-                    name="acat", value="<img alt='a picture of a cat'/>"
-                )
-                insert_route(path="/cat/picture/", node_id=catimg)
+                    catimg = insert_node(
+                        name="acat", value="<img alt='a picture of a cat'/>"
+                    )
+                    insert_route(path="/cat/picture/", node_id=catimg)
 
-                a = insert_node(
-                    name="simplefilename", value="imasimplefilewithunicode.txt"
-                )
-                apage = insert_node(name="apage", value=None)
-                insert_node_node(node_id=apage, target_node_id=a)
-                insert_route(path="/a/", node_id=apage)
-                add_template_for_node("template.html", apage)
+                    a = insert_node(
+                        name="simplefilename", value="imasimplefilewithunicode.txt"
+                    )
+                    apage = insert_node(name="apage", value=None)
+                    insert_node_node(node_id=apage, target_node_id=a)
+                    insert_route(path="/a/", node_id=apage)
+                    add_template_for_node("template.html", apage)
 
                 rv = c.get("/a/", follow_redirects=True)
                 assert bytes("Àрpĺè", "utf-8") in rv.data
 
                 assert b"<img alt='a picture of a cat'/>" in rv.data
                 assert b"[chill route /cat/picture/ ]" not in rv.data
 
@@ -1133,121 +1487,123 @@
 <ol>
 <li>apples</li>
 <li>oranges</li>
 <li>pears</li>
 </ol>
 <p>The rain---not the reign---in
 Spain.</p>"""
-        f = open(os.path.join(self.tmp_template_dir, "imasimplefile.md"), "w")
-        f.write(md)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "template.html"), "w")
-        f.write(
-            """
-          {{ simplefilename|readfile|markdown }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "imasimplefile.md"), "w") as f:
+            f.write(md)
+
+        with open(os.path.join(self.tmp_template_dir, "template.html"), "w") as f:
+            f.write(
+                """
+              {{ simplefilename|readfile|markdown }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                a = insert_node(name="simplefilename", value="imasimplefile.md")
-                apage = insert_node(name="apage", value=None)
-                insert_node_node(node_id=apage, target_node_id=a)
-                insert_route(path="/a/", node_id=apage)
-                add_template_for_node("template.html", apage)
+                db = get_db()
+                with db:
+                    init_db()
+                    a = insert_node(name="simplefilename", value="imasimplefile.md")
+                    apage = insert_node(name="apage", value=None)
+                    insert_node_node(node_id=apage, target_node_id=a)
+                    insert_route(path="/a/", node_id=apage)
+                    add_template_for_node("template.html", apage)
 
                 rv = c.get("/a/", follow_redirects=True)
                 # self.app.logger.debug('data: %s', rv.data.decode('utf-8'))
                 # self.app.logger.debug('html: %s', html)
                 assert bytes(html, "utf-8") in rv.data
 
 
 class ShortcodeRoute(ChillTestCase):
     def test_route(self):
         "Expand the route shortcode"
 
-        f = open(os.path.join(self.tmp_template_dir, "simple.html"), "w")
-        f.write(
-            """
-          <!doctype html>
-          <html><head><title>test</title></head>
-          <body>
-          <div>
-          {{ cat|shortcodes }}
-          </div>
-          </body>
-          </html>
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "simple.html"), "w") as f:
+            f.write(
+                """
+              <!doctype html>
+              <html><head><title>test</title></head>
+              <body>
+              <div>
+              {{ cat|shortcodes }}
+              </div>
+              </body>
+              </html>
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-
-                page = insert_node(name="page", value=None)
-                insert_route(path="/", node_id=page)
-                add_template_for_node("simple.html", page)
+                db = get_db()
+                with db:
+                    init_db()
+
+                    page = insert_node(name="page", value=None)
+                    insert_route(path="/", node_id=page)
+                    add_template_for_node("simple.html", page)
 
-                catimg = insert_node(
-                    name="acat", value="<img alt='a picture of a cat'/>"
-                )
-                insert_route(path="/cat/picture/", node_id=catimg)
+                    catimg = insert_node(
+                        name="acat", value="<img alt='a picture of a cat'/>"
+                    )
+                    insert_route(path="/cat/picture/", node_id=catimg)
 
-                text = "something [chill route /cat/picture/ ] [blah blah[chill route /dog/pic] the end"
-                textnode = insert_node(name="cat", value=text)
+                    text = "something [chill route /cat/picture/ ] [blah blah[chill route /dog/pic] the end"
+                    textnode = insert_node(name="cat", value=text)
 
-                insert_node_node(node_id=page, target_node_id=textnode)
+                    insert_node_node(node_id=page, target_node_id=textnode)
 
                 rv = c.get("/", follow_redirects=True)
                 assert (
                     b"something <img alt='a picture of a cat'/> [blah blah<!-- 404 '/dog/pic' --> the end"
                     in rv.data
                 )
                 assert b"[chill route /cat/picture/ ]" not in rv.data
 
                 rv = c.get("/cat/picture/", follow_redirects=True)
                 assert b"<img alt='a picture of a cat'/>" in rv.data
 
     def test_route_with_unicode(self):
         "Expand the route shortcode with unicode contents"
 
-        f = open(os.path.join(self.tmp_template_dir, "simple.html"), "w")
-        f.write(
-            """
-          <!doctype html>
-          <html><head><title>test</title></head>
-          <body>
-          <div>
-          {{ cat|shortcodes }}
-          </div>
-          </body>
-          </html>
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "simple.html"), "w") as f:
+            f.write(
+                """
+              <!doctype html>
+              <html><head><title>test</title></head>
+              <body>
+              <div>
+              {{ cat|shortcodes }}
+              </div>
+              </body>
+              </html>
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                page = insert_node(name="page", value=None)
-                insert_route(path="/", node_id=page)
-                add_template_for_node("simple.html", page)
+                    page = insert_node(name="page", value=None)
+                    insert_route(path="/", node_id=page)
+                    add_template_for_node("simple.html", page)
 
-                catimg = insert_node(name="acat", value=u"Àрpĺè")
-                insert_route(path="/cat/picture/", node_id=catimg)
+                    catimg = insert_node(name="acat", value=u"Àрpĺè")
+                    insert_route(path="/cat/picture/", node_id=catimg)
 
-                text = "something [chill route /cat/picture/ ] [blah blah[chill route /dog/pic] the end"
-                textnode = insert_node(name="cat", value=text)
+                    text = "something [chill route /cat/picture/ ] [blah blah[chill route /dog/pic] the end"
+                    textnode = insert_node(name="cat", value=text)
 
-                insert_node_node(node_id=page, target_node_id=textnode)
+                    insert_node_node(node_id=page, target_node_id=textnode)
 
                 rv = c.get("/", follow_redirects=True)
                 assert (
                     bytes(
                         "something Àрpĺè [blah blah<!-- 404 '/dog/pic' --> the end",
                         "utf-8",
                     )
@@ -1259,44 +1615,45 @@
                 assert bytes("Àрpĺè", "utf-8") in rv.data
 
 
 class ShortcodePageURI(ChillTestCase):
     def test_page_uri(self):
         "Expand the page_uri shortcode"
 
-        f = open(os.path.join(self.tmp_template_dir, "simple.html"), "w")
-        f.write(
-            """
-          <!doctype html>
-          <html><head><title>test</title></head>
-          <body>
-          <div>
-          {{ cat|shortcodes }}
-          </div>
-          </body>
-          </html>
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "simple.html"), "w") as f:
+            f.write(
+                """
+              <!doctype html>
+              <html><head><title>test</title></head>
+              <body>
+              <div>
+              {{ cat|shortcodes }}
+              </div>
+              </body>
+              </html>
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                page = insert_node(name="page", value=None)
-                insert_route(path="/", node_id=page)
-                add_template_for_node("simple.html", page)
+                    page = insert_node(name="page", value=None)
+                    insert_route(path="/", node_id=page)
+                    add_template_for_node("simple.html", page)
 
-                catpage = insert_node(name="acat", value="a page for cat")
-                insert_route(path="/cat/", node_id=catpage)
+                    catpage = insert_node(name="acat", value="a page for cat")
+                    insert_route(path="/cat/", node_id=catpage)
 
-                text = "something link for cat page that does exist = '[chill page_uri cat ]' link for dog that does not exist = '[chill page_uri dog]'"
-                textnode = insert_node(name="cat", value=text)
+                    text = "something link for cat page that does exist = '[chill page_uri cat ]' link for dog that does not exist = '[chill page_uri dog]'"
+                    textnode = insert_node(name="cat", value=text)
 
-                insert_node_node(node_id=page, target_node_id=textnode)
+                    insert_node_node(node_id=page, target_node_id=textnode)
 
                 rv = c.get("/", follow_redirects=True)
                 assert (
                     b"something link for cat page that does exist = '/cat/' link for dog that does not exist = '/dog/'"
                     in rv.data
                 )
                 assert b"[chill page_uri cat ]" not in rv.data
@@ -1306,52 +1663,51 @@
 
                 rv = c.get("/dog/", follow_redirects=True)
                 assert 404 == rv.status_code
 
 
 class PostMethod(ChillTestCase):
     def test_a(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w")
-        f.write(
-            """
-          insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select * from Llama
-          where llama_name = :llama_name;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w") as f:
+            f.write(
+                """
+              insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                db.execute(
-                    text(
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table Llama (
-                  llama_name varchar(255),
-                  location varchar(255),
-                  description text
-                  );
-                """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
                     )
-                )
+                    cur.close()
 
-                llamas_id = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/", node_id=llamas_id, weight=1, method="POST"
-                )
-                insert_query(name="insert_llama.sql", node_id=llamas_id)
+                    llamas_id = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/", node_id=llamas_id, weight=1, method="POST"
+                    )
+                    insert_query(name="insert_llama.sql", node_id=llamas_id)
 
                 llama_1 = {
                     "llama_name": "Rocky",
                     "location": "unknown",
                     "description": "first llama",
                 }
                 rv = c.post("/api/llamas/", data=llama_1)
@@ -1361,232 +1717,298 @@
                     "llama_name": "Nocky",
                     "location": "unknown",
                     "description": "second llama",
                 }
                 rv = c.post("/api/llamas/", data=llama_2)
                 assert 201 == rv.status_code
 
-                select_llama = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=select_llama,
-                    weight=1,
-                )
-                insert_query(name="select_llama.sql", node_id=select_llama)
+                with db:
+                    select_llama = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=select_llama,
+                        weight=1,
+                    )
+                    insert_query(name="select_llama.sql", node_id=select_llama)
 
                 rv = c.get("/api/llamas/name/Rocky/", follow_redirects=True)
                 rv_json = json.loads(rv.data)
                 assert set(llama_1.keys()) == set(rv_json.keys())
                 assert set(llama_1.values()) == set(rv_json.values())
 
                 rv = c.get("/api/llamas/name/Nocky/", follow_redirects=True)
                 rv_json = json.loads(rv.data)
                 assert set(llama_2.keys()) == set(rv_json.keys())
                 assert set(llama_2.values()) == set(rv_json.values())
 
+    def test_replace_of_method_value(self):
+        """The 'method' value is not able to be changed in chill."""
+        with open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w") as f:
+            f.write(
+                """
+                insert into Llama (llama_name, location, description, method) values (:llama_name, :location, :description, :method);
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
+
+        with self.app.app_context():
+            with self.app.test_client() as c:
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    # The database table has a 'method' column which will not be
+                    # compatible with chill and the current insert_llama.sql
+                    # query.
+                    cur.execute(
+                        """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text,
+                      method varchar(255)
+                      );
+                    """
+                    )
+                    cur.close()
+
+                    llamas_id = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/", node_id=llamas_id, weight=1, method="POST"
+                    )
+                    insert_query(name="insert_llama.sql", node_id=llamas_id)
+
+                llama_1 = {
+                    "llama_name": "Rocky",
+                    "location": "unknown",
+                    "description": "first llama",
+                    "method": "Tie llama to POST",
+                }
+                rv = c.post("/api/llamas/", data=llama_1)
+                assert 400 == rv.status_code
+
+                llama_2 = {
+                    "llama_name": "Nocky",
+                    "location": "unknown",
+                    "description": "second llama",
+                    "method": "POST",
+                }
+                rv = c.post("/api/llamas/", data=llama_2)
+                assert 400 == rv.status_code
+
+                llama_3 = {
+                    "llama_name": "Nocky",
+                    "location": "unknown",
+                    "description": "second llama",
+                    "method": "GET",
+                }
+                rv = c.post("/api/llamas/", data=llama_3)
+                assert 400 == rv.status_code
+
 
 class PutMethod(ChillTestCase):
     def test_a(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w")
-        f.write(
-            """
-          insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select * from Llama
-          where llama_name = :llama_name;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w") as f:
+            f.write(
+                """
+              insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                db.execute(
-                    text(
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table Llama (
-                  llama_name varchar(255),
-                  location varchar(255),
-                  description text
-                  );
-                """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
                     )
-                )
+                    cur.close()
 
-                llamas_id = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=llamas_id,
-                    weight=1,
-                    method="PUT",
-                )
-                insert_query(name="insert_llama.sql", node_id=llamas_id)
+                    llamas_id = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=llamas_id,
+                        weight=1,
+                        method="PUT",
+                    )
+                    insert_query(name="insert_llama.sql", node_id=llamas_id)
 
                 llama_1 = {
                     "llama_name": "Socky",
                     "location": "unknown",
                     "description": "first llama",
                 }
                 rv = c.put("/api/llamas/name/Socky/", data=llama_1)
                 assert 201 == rv.status_code
 
-                select_llama = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=select_llama,
-                    weight=1,
-                )
-                insert_query(name="select_llama.sql", node_id=select_llama)
+                with db:
+                    select_llama = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=select_llama,
+                        weight=1,
+                    )
+                    insert_query(name="select_llama.sql", node_id=select_llama)
 
                 rv = c.get("/api/llamas/name/Socky/", follow_redirects=True)
                 rv_json = json.loads(rv.data)
                 assert set(llama_1.keys()) == set(rv_json.keys())
                 assert set(llama_1.values()) == set(rv_json.values())
 
 
 class PatchMethod(ChillTestCase):
     def test_a(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "update_llama.sql"), "w")
-        f.write(
-            """
-          update Llama set location = :location, description = :description where llama_name = :llama_name;
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select * from Llama
-          where llama_name = :llama_name;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "update_llama.sql"), "w") as f:
+            f.write(
+                """
+              update Llama set location = :location, description = :description where llama_name = :llama_name;
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                db.execute(
-                    text(
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table Llama (
-                  llama_name varchar(255),
-                  location varchar(255),
-                  description text
-                  );
-                """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
                     )
-                )
 
-                db.execute(
-                    text(
+                    cur.execute(
                         """
-                  insert into Llama (llama_name) values ('Pocky');
-                """
+                      insert into Llama (llama_name) values ('Pocky');
+                    """
                     )
-                )
+                    cur.close()
 
-                llamas_id = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=llamas_id,
-                    weight=1,
-                    method="PATCH",
-                )
-                insert_query(name="update_llama.sql", node_id=llamas_id)
+                    llamas_id = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=llamas_id,
+                        weight=1,
+                        method="PATCH",
+                    )
+                    insert_query(name="update_llama.sql", node_id=llamas_id)
 
                 llama_1 = {
                     "llama_name": "Pocky",
                     "location": "unknown",
                     "description": "first llama",
                 }
                 rv = c.patch("/api/llamas/name/Pocky/", data=llama_1)
                 assert 201 == rv.status_code
 
-                select_llama = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=select_llama,
-                    weight=1,
-                )
-                insert_query(name="select_llama.sql", node_id=select_llama)
+                with db:
+                    select_llama = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=select_llama,
+                        weight=1,
+                    )
+                    insert_query(name="select_llama.sql", node_id=select_llama)
 
                 rv = c.get("/api/llamas/name/Pocky/", follow_redirects=True)
                 rv_json = json.loads(rv.data)
                 assert set(llama_1.keys()) == set(rv_json.keys())
                 assert set(llama_1.values()) == set(rv_json.values())
 
 
 class DeleteMethod(ChillTestCase):
     def test_a(self):
-        """
-        """
-        f = open(os.path.join(self.tmp_template_dir, "delete_llama.sql"), "w")
-        f.write(
-            """
-          Delete from Llama where llama_name = :llama_name;
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select * from Llama
-          where llama_name = :llama_name;
-          """
-        )
-        f.close()
+        """ """
+        with open(os.path.join(self.tmp_template_dir, "delete_llama.sql"), "w") as f:
+            f.write(
+                """
+              Delete from Llama where llama_name = :llama_name;
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                db.execute(
-                    text(
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table Llama (
-                  llama_name varchar(255),
-                  location varchar(255),
-                  description text
-                  );
-                """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
                     )
-                )
 
-                db.execute(
-                    text(
+                    cur.execute(
                         """
-                  insert into Llama (llama_name, location, description) values ('Docky', 'somewhere', 'damaged');
-                """
+                      insert into Llama (llama_name, location, description) values ('Docky', 'somewhere', 'damaged');
+                    """
                     )
-                )
+                    cur.close()
 
-                select_llama = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=select_llama,
-                    weight=1,
-                )
-                insert_query(name="select_llama.sql", node_id=select_llama)
+                    select_llama = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=select_llama,
+                        weight=1,
+                    )
+                    insert_query(name="select_llama.sql", node_id=select_llama)
 
-                llamas_id = insert_node(name="llamas", value=None)
-                insert_route(
-                    path="/api/llamas/name/<llama_name>/",
-                    node_id=llamas_id,
-                    weight=1,
-                    method="DELETE",
-                )
-                insert_query(name="delete_llama.sql", node_id=llamas_id)
+                    llamas_id = insert_node(name="llamas", value=None)
+                    insert_route(
+                        path="/api/llamas/name/<llama_name>/",
+                        node_id=llamas_id,
+                        weight=1,
+                        method="DELETE",
+                    )
+                    insert_query(name="delete_llama.sql", node_id=llamas_id)
 
                 rv = c.get("/api/llamas/name/Docky/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 rv = c.delete("/api/llamas/name/Docky/")
                 assert 204 == rv.status_code
 
@@ -1602,15 +2024,15 @@
         with open(test_dump_file, "r") as f:
             contents = f.read()
             self.app.logger.debug("contents {}".format(contents))
             self.app.logger.debug("expected {}".format(expected_chill_nodes))
             documents = yaml.safe_load_all(contents)
             for item in documents:
                 self.app.logger.debug("check_dump {}".format(item))
-                assert isinstance(item, ChillNode) == True
+                assert isinstance(item, ChillNode) is True
 
                 if isinstance(expected_chill_nodes, list):
                     match = expected_chill_nodes.pop(
                         expected_chill_nodes.index(str(item))
                     )
                     assert match == str(item)
 
@@ -1624,21 +2046,22 @@
 route: /simple/
 value: "simple string value"
         """
         expected_chill_nodes = [
             "ChillNode(name='simple_value_at_route', value='simple string value', template=None, route='/simple/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/simple/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -1662,21 +2085,22 @@
 value: "another string value"
         """
         expected_chill_nodes = [
             "ChillNode(name='simple_value_at_route', value='simple string value', template=None, route='/simple/')",
             "ChillNode(name='another_value_at_route', value='another string value', template=None, route='/another/')",
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/simple/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -1700,25 +2124,25 @@
 route: /total-count/
 value: get-total-count.sql
         """
         expected_chill_nodes = [
             "ChillNode(name='query_value_at_route', value='get-total-count.sql', template=None, route='/total-count/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "get-total-count.sql"), "w")
-        f.write("""select 26 as count;""")
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "get-total-count.sql"), "w") as f:
+            f.write("""select 26 as count;""")
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/total-count/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -1746,48 +2170,47 @@
 value: select_llama.sql
         """
         expected_chill_nodes = [
             "ChillNode(name='llamas', value='insert_llama.sql', template=None, route={'method': 'POST', 'path': '/api/llamas/'})",
             "ChillNode(name='llamas', value='select_llama.sql', template=None, route='/api/llamas/name/<llama_name>/')",
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w")
-        f.write(
-            """
-          insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w")
-        f.write(
-            """
-          select * from Llama
-          where llama_name = :llama_name;
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "insert_llama.sql"), "w") as f:
+            f.write(
+                """
+              insert into Llama (llama_name, location, description) values (:llama_name, :location, :description);
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "select_llama.sql"), "w") as f:
+            f.write(
+                """
+              select * from Llama
+              where llama_name = :llama_name;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
-                db.execute(
-                    text(
+                db = get_db()
+                with db:
+                    init_db()
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table Llama (
-                  llama_name varchar(255),
-                  location varchar(255),
-                  description text
-                  );
-                """
+                    create table Llama (
+                      llama_name varchar(255),
+                      location varchar(255),
+                      description text
+                      );
+                    """
                     )
-                )
+                    cur.close()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 llama_1 = {
                     "llama_name": "Rocky",
                     "location": "unknown",
                     "description": "first llama",
@@ -1827,30 +2250,30 @@
 template: test.html
 value: "simple"
         """
         expected_chill_nodes = [
             "ChillNode(name='simple_value_at_route', value='simple', template='test.html', route='/simple-template/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "test.html"), "w")
-        f.write(
-            """
-          <h1>test template</h1>
-          {{ value }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "test.html"), "w") as f:
+            f.write(
+                """
+              <h1>test template</h1>
+              {{ value }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/simple-template/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -1870,21 +2293,22 @@
 value:
     content: "hello"
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'content': 'hello'}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -1904,21 +2328,22 @@
     content:
         chill_value: "hello"
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'content': 'hello'}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -1935,21 +2360,22 @@
 name: page
 route: /
 # Boolean values like Yes, No, true, False are not supported. Use a string value
 # like 'Yes' or 'false'.
 value: Yes
         """
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 try:
                     load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
                 except TypeError as err:
                     self.app.logger.debug(err)
 
                 rv = c.get("/", follow_redirects=True)
@@ -1965,21 +2391,22 @@
 route: /
 # Boolean values like Yes, No, true, False are not supported. Use a string value
 # like 'Yes' or 'false'.
 value:
     content: yes
         """
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 try:
                     load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
                 except TypeError as err:
                     self.app.logger.debug(err)
 
                 rv = c.get("/", follow_redirects=True)
@@ -1996,21 +2423,22 @@
 # Boolean values like Yes, No, true, False are not supported. Use a string value
 # like 'Yes' or 'false'.
 value:
     - yes
     - no
         """
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 try:
                     load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
                 except TypeError as err:
                     self.app.logger.debug(err)
 
                 rv = c.get("/", follow_redirects=True)
@@ -2025,21 +2453,22 @@
 name: page
 route: /
 value:
     content:
         chill_value: Yes
         """
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 try:
                     load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
                 except TypeError as err:
                     self.app.logger.debug(err)
 
                 rv = c.get("/", follow_redirects=True)
@@ -2055,21 +2484,22 @@
 route: /
 value: None
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value='None', template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 try:
                     load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
                 except TypeError as err:
                     self.app.logger.debug(err)
 
                 rv = c.get("/", follow_redirects=True)
@@ -2089,21 +2519,22 @@
     content: "hello"
     title: "a title here"
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'content': 'hello', 'title': 'a title here'}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2128,21 +2559,22 @@
     - 'Yes'
     - 'No'
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value=[{'value': 'a is for aardvark'}, {'value': 'b is for bat'}, {'value': 'c is for cat'}, {'value': '1234'}, {'value': 'Yes'}, {'value': 'No'}], template=None, route='/list/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/list/", follow_redirects=True)
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
                 assert 200 == rv.status_code
 
@@ -2174,21 +2606,22 @@
     - "c is for cat"
     - 1234
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value=[{'value': 'a is for aardvark'}, {'value': {'page': {'bottom': 'No', 'menu': [{'menu': 'one'}, {'menu': 'two'}], 'top': 'Yes'}}}, {'value': 'c is for cat'}, {'value': '1234'}], template=None, route='/list/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/list/", follow_redirects=True)
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
                 assert 200 == rv.status_code
 
@@ -2230,21 +2663,22 @@
                 two: 'puppy'
                 three: 'tadpole'
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'page': {'content': 'an-example-doc.html', 'description': 'Description would go here and can be multiple lines.\\n', 'menu': {'footer': {'one': 'kitten', 'three': 'tadpole', 'two': 'puppy'}, 'one': 'cat', 'two': 'dog'}, 'menu2': {'footer': {'one': 'kitten', 'three': 'tadpole', 'two': 'puppy'}, 'one': 'cat', 'two': 'dog'}, 'title': 'a title here'}}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2272,37 +2706,35 @@
     best: get-best-animal.sql
     simple: simple.sql
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'best': 'get-best-animal.sql', 'simple': 'simple.sql', 'total_count': 'get-total-count.sql'}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "get-total-count.sql"), "w")
-        f.write("""select 26 as value;""")
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "get-best-animal.sql"), "w")
-        f.write("""select 'kangaroo' as value;""")
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "simple.sql"), "w")
-        f.write(
-            """
-          select 'yup' as a, 'pretty' as b, 'darn' as c, 'simple' as d;
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "get-total-count.sql"), "w") as f:
+            f.write("""select 26 as value;""")
+
+        with open(os.path.join(self.tmp_template_dir, "get-best-animal.sql"), "w") as f:
+            f.write("""select 'kangaroo' as value;""")
+
+        with open(os.path.join(self.tmp_template_dir, "simple.sql"), "w") as f:
+            f.write(
+                """
+              select 'yup' as a, 'pretty' as b, 'darn' as c, 'simple' as d;
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2337,29 +2769,28 @@
                 three: 'tadpole'
                 best: get-best-animal.sql
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'page': {'description': 'Description would go here and can be multiple lines.\\n', 'menu': {'footer': {'best': 'get-best-animal.sql', 'one': 'kitten', 'three': 'tadpole', 'two': 'puppy'}, 'one': 'cat', 'two': 'dog'}, 'title': 'a title here', 'total_count': 'get-total-count.sql'}}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "get-total-count.sql"), "w")
-        f.write("""select 26 as value;""")
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "get-best-animal.sql"), "w")
-        f.write("""select 'kangaroo' as value;""")
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "get-total-count.sql"), "w") as f:
+            f.write("""select 26 as value;""")
+
+        with open(os.path.join(self.tmp_template_dir, "get-best-animal.sql"), "w") as f:
+            f.write("""select 'kangaroo' as value;""")
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2388,52 +2819,48 @@
 route: /
 value: get-list-of-animals.sql
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value='get-list-of-animals.sql', template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "get-list-of-animals.sql"), "w")
-        f.write("""select name, description from Animal;""")
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(
+            os.path.join(self.tmp_template_dir, "get-list-of-animals.sql"), "w"
+        ) as f:
+            f.write("""select name, description from Animal;""")
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
-                db.execute(
-                    text(
+                    cur = db.cursor()
+                    cur.execute(
                         """
-                create table Animal (
-                  id integer,
-                  name varchar(30),
-                  description text
-                  );
-                """
+                    create table Animal (
+                      id integer,
+                      name varchar(30),
+                      description text
+                      );
+                    """
                     )
-                )
-                db.execute(
-                    text(
+                    cur.execute(
                         "insert into Animal (name, description) values ('horse', '4 legged furry thing');"
                     )
-                )
-                db.execute(
-                    text(
+                    cur.execute(
                         "insert into Animal (name, description) values ('llama', 'furry thing with four legs');"
                     )
-                )
-                db.execute(
-                    text(
+                    cur.execute(
                         "insert into Animal (name, description) values ('cow', 'a furry thing that also has 4 legs');"
                     )
-                )
+                    cur.close()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2456,30 +2883,30 @@
         chill_value: "hello"
         chill_template: "hello.html"
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'content': {'chill_template': 'hello.html', 'chill_value': 'hello'}}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "hello.html"), "w")
-        f.write(
-            """
-          <h1>greeting template</h1>
-          {{ value }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "hello.html"), "w") as f:
+            f.write(
+                """
+              <h1>greeting template</h1>
+              {{ value }}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2499,29 +2926,29 @@
     content:
         chill_template: "hello.html"
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'content': {'chill_template': 'hello.html'}}, template=None, route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "hello.html"), "w")
-        f.write(
-            """
-          <h1>greeting template</h1>
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
+
+        with open(os.path.join(self.tmp_template_dir, "hello.html"), "w") as f:
+            f.write(
+                """
+              <h1>greeting template</h1>
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
@@ -2554,63 +2981,59 @@
                     - subitem: "ee"
                 chill_template: three.html
         """
         expected_chill_nodes = [
             "ChillNode(name='page', value={'content': {'chill_template': 'hello.html', 'chill_value': [{'content': {'item': {'chill_template': 'one.html', 'chill_value': 'one'}}}, {'content': {'item': {'chill_template': 'two.html', 'chill_value': 'two'}}}, {'content': {'item': {'chill_template': 'three.html', 'chill_value': [{'item': {'subitem': 'thr'}}, {'item': {'subitem': 'ee'}}]}}}]}}, template='page.html', route='/')"
         ]
 
-        f = open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w")
-        f.write(yaml_content)
-        f.close()
-
-        f = open(os.path.join(self.tmp_template_dir, "page.html"), "w")
-        f.write(
-            """
-          page
-          {{ content|safe }}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "test-data.yaml"), "w") as f:
+            f.write(yaml_content)
 
-        f = open(os.path.join(self.tmp_template_dir, "hello.html"), "w")
-        f.write(
-            """
-          <h1>greeting template</h1>
-          {% for item in value %}
-          {{ item.content.item|safe }}
-          {% endfor %}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "page.html"), "w") as f:
+            f.write(
+                """
+              page
+              {{ content|safe }}
+              """
+            )
 
-        f = open(os.path.join(self.tmp_template_dir, "one.html"), "w")
-        f.write(
-            """
-            <span>First</span> {{ value }}
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "two.html"), "w")
-        f.write(
-            """
-            <span>Second</span> {{ value }}
-          """
-        )
-        f.close()
-        f = open(os.path.join(self.tmp_template_dir, "three.html"), "w")
-        f.write(
-            """
-            <span>Third</span> {% for item in value -%} {{ item.item.subitem }}{%- endfor %}
-          """
-        )
-        f.close()
+        with open(os.path.join(self.tmp_template_dir, "hello.html"), "w") as f:
+            f.write(
+                """
+              <h1>greeting template</h1>
+              {% for item in value %}
+              {{ item.content.item|safe }}
+              {% endfor %}
+              """
+            )
+
+        with open(os.path.join(self.tmp_template_dir, "one.html"), "w") as f:
+            f.write(
+                """
+                <span>First</span> {{ value }}
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "two.html"), "w") as f:
+            f.write(
+                """
+                <span>Second</span> {{ value }}
+              """
+            )
+        with open(os.path.join(self.tmp_template_dir, "three.html"), "w") as f:
+            f.write(
+                """
+                <span>Third</span> {% for item in value -%} {{ item.item.subitem }}{%- endfor %}
+              """
+            )
 
         with self.app.app_context():
             with self.app.test_client() as c:
-                init_db()
+                db = get_db()
+                with db:
+                    init_db()
 
                 load_yaml(os.path.join(self.tmp_template_dir, "test-data.yaml"))
 
                 rv = c.get("/", follow_redirects=True)
                 assert 200 == rv.status_code
 
                 self.app.logger.debug("data: %s", rv.data.decode("utf-8"))
```

### Comparing `chill-0.8.1/src/chill/yaml_chill_node.py` & `chill-0.9.0/src/chill/yaml_chill_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,275 +1,358 @@
 import os
-import sqlite3
 
-from sqlalchemy.sql import text
 from flask import current_app
 import yaml
 
-from chill.app import make_app, db
 from chill.database import (
-        init_db,
-        insert_node,
-        insert_node_node,
-        delete_node,
-        select_node,
-        insert_route,
-        insert_query,
-        add_template_for_node,
-        fetch_query_string,
-        rowify,
-        )
+    get_db,
+    insert_node,
+    insert_node_node,
+    select_node,
+    insert_route,
+    insert_query,
+    add_template_for_node,
+    fetch_query_string,
+)
+
 
 def _is_sql_file(file_name):
-    folder = current_app.config.get('THEME_SQL_FOLDER')
+    folder = current_app.config.get("THEME_SQL_FOLDER")
     file_path = os.path.join(folder, file_name)
     return os.path.isfile(file_path)
 
+
 def _is_template_file(file_name):
-    folder = current_app.config.get('THEME_TEMPLATE_FOLDER')
+    folder = current_app.config.get("THEME_TEMPLATE_FOLDER")
     file_path = os.path.join(folder, file_name)
     return os.path.isfile(file_path)
 
+
 def _value_is_simple_string(value):
     if isinstance(value, str):
         _value = value.strip()
-        if _value.endswith('.sql') and _is_sql_file(_value):
+        if _value.endswith(".sql") and _is_sql_file(_value):
             return False
         else:
             return True
 
+
 def _add_node_to_parent(parent_node_id, name, value):
     node_has_template = False
     if isinstance(value, bool):
-        raise TypeError('Boolean values are not supported. Surround the value with quotes to set as string.')
+        raise TypeError(
+            "Boolean values are not supported. Surround the value with quotes to set as string."
+        )
     _value = value
     if isinstance(value, int) or isinstance(value, float):
         _value = str(value)
-    elif isinstance(value, dict) and set(value.keys()).issubset({'chill_template', 'chill_value'}):
-        if value.get('chill_template') == None:
-            _add_node_to_parent(parent_node_id, name, value.get('chill_value'))
+    elif isinstance(value, dict) and set(value.keys()).issubset(
+        {"chill_template", "chill_value"}
+    ):
+        if value.get("chill_template") is None:
+            _add_node_to_parent(parent_node_id, name, value.get("chill_value"))
             return
         else:
-            _value = value.get('chill_value')
+            _value = value.get("chill_value")
             if isinstance(_value, int) or isinstance(_value, float):
                 _value = str(_value)
             node_has_template = True
 
     item_node_id = None
     if _value_is_simple_string(_value):
         item_node_id = insert_node(name=name, value=_value)
-        insert_query(name='select_link_node_from_node.sql', node_id=item_node_id)
+        insert_query(name="select_link_node_from_node.sql", node_id=item_node_id)
         insert_node_node(node_id=parent_node_id, target_node_id=item_node_id)
 
     elif isinstance(_value, str) and _is_sql_file(_value):
         item_node_id = insert_node(name=name, value=None)
         insert_query(name=_value, node_id=item_node_id)
         insert_node_node(node_id=parent_node_id, target_node_id=item_node_id)
 
     else:
         item_node_id = insert_node(name=name, value=None)
-        insert_query(name='select_link_node_from_node.sql', node_id=item_node_id)
+        insert_query(name="select_link_node_from_node.sql", node_id=item_node_id)
         insert_node_node(node_id=parent_node_id, target_node_id=item_node_id)
 
         if isinstance(_value, dict):
-            if set(_value.keys()).issubset({'chill_template', 'chill_value'}):
-                raise TypeError("chill_template or chill_value should not be set directly under a chill_value")
+            if set(_value.keys()).issubset({"chill_template", "chill_value"}):
+                raise TypeError(
+                    "chill_template or chill_value should not be set directly under a chill_value"
+                )
             for item_name in _value.keys():
                 item_value = _value.get(item_name)
                 _add_node_to_parent(item_node_id, item_name, item_value)
 
         elif isinstance(_value, list):
             for item_value in _value:
                 _add_node_to_parent(item_node_id, name, item_value)
         elif _value == None:
             pass
         else:
-            raise TypeError('unsupported value type. Use only dict, or list.')
+            raise TypeError("unsupported value type. Use only dict, or list.")
 
     if node_has_template:
-        add_template_for_node(value.get('chill_template'), item_node_id)
+        add_template_for_node(value.get("chill_template"), item_node_id)
+
 
 def _render_chill_node_value(node_id, root=False):
     # get the node
-    query_result = db.execute(text(fetch_query_string('select_query_from_node.sql')), {"node_id": node_id}).fetchall()
+    db = get_db()
+    cur = db.cursor()
+    query_result = cur.execute(
+        fetch_query_string("select_query_from_node.sql"), {"node_id": node_id}
+    ).fetchall()
     value = None
     if query_result:
-        #current_app.logger.debug('render {node_id}'.format(node_id=node_id))
-        #current_app.logger.debug(query_result)
+        # current_app.logger.debug('render {node_id}'.format(node_id=node_id))
+        # current_app.logger.debug(query_result)
         values = []
         if len(query_result) > 1:
-            raise NotImplementedError('TODO: Support for multiple queries found for a node.')
-        for query_name in [x['name'] for x in query_result]:
-            if query_name == 'select_link_node_from_node.sql':
-                link_nodes_result = db.execute(text(fetch_query_string('select_link_node_from_node.sql')), {"node_id": node_id}).fetchall()
+            raise NotImplementedError(
+                "TODO: Support for multiple queries found for a node."
+            )
+        for query_name in [x["name"] for x in query_result]:
+            if query_name == "select_link_node_from_node.sql":
+                link_nodes_result = cur.execute(
+                    fetch_query_string("select_link_node_from_node.sql"),
+                    {"node_id": node_id},
+                ).fetchall()
                 if link_nodes_result:
                     value = {}
-                    if len(link_nodes_result) > 1 and link_nodes_result[0].name == link_nodes_result[1].name:
+                    if (
+                        len(link_nodes_result) > 1
+                        and link_nodes_result[0]["name"] == link_nodes_result[1]["name"]
+                    ):
                         value = []
                         for link_node in link_nodes_result:
                             item = {}
-                            item[link_node.name] = _render_chill_node_value(link_node.node_id)
+                            item[link_node["name"]] = _render_chill_node_value(
+                                link_node["node_id"]
+                            )
                             value.append(item)
                     else:
                         for link_node in link_nodes_result:
-                            value[link_node.name] = _render_chill_node_value(link_node.node_id)
+                            value[link_node["name"]] = _render_chill_node_value(
+                                link_node["node_id"]
+                            )
 
                 else:
                     node = select_node(node_id=node_id)[0]
-                    value = node.value
+                    value = node["value"]
             else:
                 value = query_name
     else:
         node = select_node(node_id=node_id)[0]
-        value = node.value
+        value = node["value"]
 
     if not root:
-        template_for_node_result = db.execute(text(fetch_query_string('select_template_from_node.sql')), {"node_id": node_id}).fetchone()
+        template_for_node_result = cur.execute(
+            fetch_query_string("select_template_from_node.sql"), {"node_id": node_id}
+        ).fetchone()
         if template_for_node_result:
-            template_for_node = template_for_node_result.name
+            template_for_node = template_for_node_result["name"]
             chill_value = value
             value = {
-                'chill_template': template_for_node,
+                "chill_template": template_for_node,
             }
             if chill_value != None:
-                value['chill_value'] = chill_value
+                value["chill_value"] = chill_value
 
+    cur.close()
     return value
 
+
 class ChillNode(yaml.YAMLObject):
     yaml_loader = yaml.SafeLoader
-    yaml_tag = u'!ChillNode'
+    yaml_tag = u"!ChillNode"
 
     # Default props
     name = None
     value = None
     template = None
     route = None
 
-    def __init__(self, name, node_id=None, value=None, template=None, query=None, path=None, method=None, weight=None):
+    def __init__(
+        self,
+        name,
+        node_id=None,
+        value=None,
+        template=None,
+        query=None,
+        path=None,
+        method=None,
+        weight=None,
+    ):
         self.name = name
-        if value != None:
+        if value is not None:
             self.value = value
-        if template != None:
+        if template is not None:
             self.template = template
-        if query != None:
-            if query == 'select_link_node_from_node.sql':
+        if query is not None:
+            if query == "select_link_node_from_node.sql":
                 self.value = _render_chill_node_value(node_id, root=True)
             else:
                 self.value = query
 
-        if path != None:
-            if isinstance(path, str) and method in (None, 'GET') and weight in (None, ''):
+        if path is not None:
+            if (
+                isinstance(path, str)
+                and method in (None, "GET")
+                and weight in (None, "")
+            ):
                 self.route = path
             else:
-                route = {
-                    "path": path
-                }
-                if method != None:
+                route = {"path": path}
+                if method is not None:
                     route["method"] = method
-                if weight != None and weight != '':
+                if weight is not None and weight != "":
                     route["weight"] = weight
                 self.route = route
 
     def load(self):
         if not self.name:
-            raise TypeError('the `name` property is required for ChillNode')
+            raise TypeError("the `name` property is required for ChillNode")
 
         if isinstance(self.value, bool):
-            raise TypeError('Boolean values are not supported. Surround the value with quotes to set as string.')
+            raise TypeError(
+                "Boolean values are not supported. Surround the value with quotes to set as string."
+            )
 
         value = None
         if _value_is_simple_string(self.value):
             value = self.value
         elif isinstance(self.value, int) or isinstance(self.value, float):
             value = str(self.value)
 
-        # Insert the chill_node
-        chill_node = insert_node(name=self.name, value=value)
-
-        # Set the route
-        if self.route:
-            if isinstance(self.route, str):
-                insert_route(path=self.route, node_id=chill_node, weight=None, method='GET')
-            elif isinstance(self.route, dict):
-                route_path = self.route.get('path', None)
-                if route_path == None:
-                    raise TypeError('A path must be set for a route')
-                elif not isinstance(route_path, str):
-                    raise TypeError('A path must be a string value')
-                route_weight = self.route.get('weight', None)
-                route_method = self.route.get('method', 'GET')
-                if route_weight != None and not isinstance(route_weight, int):
-                    raise TypeError("route weight value needs to be integer if defined")
-                if (isinstance(route_method, str) and route_method.upper() not in ('GET', 'POST', 'PUT', 'DELETE', 'PATCH')):
-                    raise TypeError("route method value needs to be 'GET', 'POST', 'PUT', 'DELETE', or 'PATCH' if defined")
-                elif not isinstance(route_method, str):
-                    raise TypeError("route method value needs to be 'GET', 'POST', 'PUT', 'DELETE', or 'PATCH' if defined")
-                insert_route(path=self.route['path'], node_id=chill_node, weight=route_weight, method=route_method.upper())
+        # Use context manager to automatically call db.commit() when successful,
+        # otherwise db.rollback() is called.
+        db = get_db()
+        with db:
+            # Insert the chill_node
+            chill_node = insert_node(name=self.name, value=value)
+
+            # Set the route
+            if self.route:
+                if isinstance(self.route, str):
+                    insert_route(
+                        path=self.route, node_id=chill_node, weight=None, method="GET"
+                    )
+                elif isinstance(self.route, dict):
+                    route_path = self.route.get("path", None)
+                    if route_path == None:
+                        raise TypeError("A path must be set for a route")
+                    elif not isinstance(route_path, str):
+                        raise TypeError("A path must be a string value")
+                    route_weight = self.route.get("weight", None)
+                    route_method = self.route.get("method", "GET")
+                    if route_weight != None and not isinstance(route_weight, int):
+                        raise TypeError("route weight value needs to be integer if defined")
+                    if isinstance(route_method, str) and route_method.upper() not in (
+                        "GET",
+                        "POST",
+                        "PUT",
+                        "DELETE",
+                        "PATCH",
+                    ):
+                        raise TypeError(
+                            "route method value needs to be 'GET', 'POST', 'PUT', 'DELETE', or 'PATCH' if defined"
+                        )
+                    elif not isinstance(route_method, str):
+                        raise TypeError(
+                            "route method value needs to be 'GET', 'POST', 'PUT', 'DELETE', or 'PATCH' if defined"
+                        )
+                    insert_route(
+                        path=self.route["path"],
+                        node_id=chill_node,
+                        weight=route_weight,
+                        method=route_method.upper(),
+                    )
 
-            else:
-                raise TypeError('route value other then str or dict not supported')
+                else:
+                    raise TypeError("route value other then str or dict not supported")
 
-        # Set the template
-        if self.template:
-            if isinstance(self.template, str):
-                if _is_template_file(self.template):
-                    add_template_for_node(name=self.template, node_id=chill_node)
+            # Set the template
+            if self.template:
+                if isinstance(self.template, str):
+                    if _is_template_file(self.template):
+                        add_template_for_node(name=self.template, node_id=chill_node)
+                    else:
+                        raise TypeError(
+                            "template value must be a path to a file in template folder"
+                        )
                 else:
-                    raise TypeError('template value must be a path to a file in template folder')
-            else:
-                raise TypeError('template value must be a string')
+                    raise TypeError("template value must be a string")
 
-        # Set the query if value is not simple string
-        if not value:
-            if isinstance(self.value, str) and _is_sql_file(self.value):
-                insert_query(name=self.value, node_id=chill_node)
-
-            elif isinstance(self.value, dict):
-                if set(self.value.keys()).issubset({'chill_template', 'chill_value'}):
-                    raise TypeError("chill_template or chill_value should not be set at the top ChillNode value.")
-                for item_name in self.value.keys():
-                    item_value = self.value.get(item_name)
-                    _add_node_to_parent(chill_node, item_name, item_value)
-
-            elif isinstance(self.value, list):
-                for item_value in self.value:
-                    _add_node_to_parent(chill_node, 'value', item_value)
-            elif self.value == None:
-                pass
-            else:
-                raise TypeError('unsupported value type. Use only dict, or list.')
+            # Set the query if value is not simple string
+            if not value:
+                if isinstance(self.value, str) and _is_sql_file(self.value):
+                    insert_query(name=self.value, node_id=chill_node)
+
+                elif isinstance(self.value, dict):
+                    if set(self.value.keys()).issubset({"chill_template", "chill_value"}):
+                        raise TypeError(
+                            "chill_template or chill_value should not be set at the top ChillNode value."
+                        )
+                    for item_name in self.value.keys():
+                        item_value = self.value.get(item_name)
+                        _add_node_to_parent(chill_node, item_name, item_value)
+
+                elif isinstance(self.value, list):
+                    for item_value in self.value:
+                        _add_node_to_parent(chill_node, "value", item_value)
+                elif self.value == None:
+                    pass
+                else:
+                    raise TypeError("unsupported value type. Use only dict, or list.")
 
     def __repr__(self):
-        return "%s(name=%r, value=%r, template=%r, route=%r)" % (self.__class__.__name__, self.name, self.value, self.template, self.route)
+        return "%s(name=%r, value=%r, template=%r, route=%r)" % (
+            self.__class__.__name__,
+            self.name,
+            self.value,
+            self.template,
+            self.route,
+        )
 
 
 def dump_yaml(yaml_file):
     "Dump chill database structure to ChillNode yaml objects."
-
-    result = db.execute(text(fetch_query_string('select_all_chill_nodes.sql'))).fetchall()
+    db = get_db()
+    cur = db.cursor()
+    result = cur.execute(fetch_query_string("select_all_chill_nodes.sql")).fetchall()
+    cur.close()
 
     node_list = result
     chill_nodes = []
 
     for node in node_list:
-        if isinstance(node.path, str):
-            chill_node = ChillNode(name=node.name, node_id=node.node_id, value=node.value, template=node.template, query=node.query, path=node.path, method=node.method, weight=node.weight)
+        if isinstance(node["path"], str):
+            chill_node = ChillNode(
+                name=node["name"],
+                node_id=node["node_id"],
+                value=node["value"],
+                template=node["template"],
+                query=node["query"],
+                path=node["path"],
+                method=node["method"],
+                weight=node["weight"],
+            )
 
             chill_nodes.append(chill_node)
 
-    with open(yaml_file, 'w') as f:
+    with open(yaml_file, "w") as f:
         yaml.dump_all(chill_nodes, stream=f, default_flow_style=False)
-        #current_app.logger.debug(yaml.dump_all(chill_nodes, default_flow_style=False))
+        # current_app.logger.debug(yaml.dump_all(chill_nodes, default_flow_style=False))
+
 
 def load_yaml(yaml_file):
     "Load ChillNode yaml objects into chill database."
 
-    with open(yaml_file, 'r') as f:
+    with open(yaml_file, "r") as f:
         documents = yaml.safe_load_all(f.read())
         for item in documents:
-            #current_app.logger.debug(item)
+            # current_app.logger.debug(item)
             if isinstance(item, ChillNode):
                 try:
                     item.load()
                 except NotImplementedError as err:
                     current_app.logger.warning(err)
```

### Comparing `chill-0.8.1/src/chill.egg-info/SOURCES.txt` & `chill-0.9.0/src/chill.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,34 @@
+.dockerignore
+.flake8
+.gitignore
+COPYING
+COPYING.LESSER
+Dockerfile
+MANIFEST.in
 README.md
+pyproject.toml
+requirements.txt
+setup.cfg
 setup.py
+docs/add-page-script.md
+docs/docker-container-usage.md
+docs/index.md
+docs/yaml_chill_node_guide_to_dump_and_load.md
+example/Dockerfile
+example/chill-data.yaml
+example/site.cfg
+example/templates/homepage.html
 src/chill/__init__.py
 src/chill/_version.py
 src/chill/api.py
 src/chill/app.py
-src/chill/cache.py
-src/chill/client.py
 src/chill/database.py
 src/chill/migrations.py
-src/chill/operate.py
 src/chill/public.py
-src/chill/pyselect.py
 src/chill/script.py
 src/chill/shortcodes.py
 src/chill/test_api.py
 src/chill/test_loader.py
 src/chill/tests.py
 src/chill/yaml_chill_node.py
 src/chill.egg-info/PKG-INFO
```

