# Comparing `tmp/dbt-duckdb-1.5.1.tar.gz` & `tmp/dbt-duckdb-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-duckdb-1.5.1.tar", last modified: Fri May  5 18:27:10 2023, max compression
+gzip compressed data, was "dbt-duckdb-1.5.2.tar", last modified: Thu Jun 22 16:53:39 2023, max compression
```

## Comparing `dbt-duckdb-1.5.1.tar` & `dbt-duckdb-1.5.2.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.598988 dbt-duckdb-1.5.1/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)    13064 2023-05-05 18:27:10.598676 dbt-duckdb-1.5.1/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)    12760 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.587737 dbt-duckdb-1.5.1/dbt/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.587956 dbt-duckdb-1.5.1/dbt/adapters/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/adapters/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.590138 dbt-duckdb-1.5.1/dbt/adapters/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       18 2023-05-05 18:17:03.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 jwills     (501) staff       (20)     3163 2023-05-03 15:42:01.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 jwills     (501) staff       (20)     6712 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/credentials.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.590911 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/
--rw-r--r--   0 jwills     (501) staff       (20)     5173 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     1900 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/buenavista.py
--rw-r--r--   0 jwills     (501) staff       (20)     3871 2023-05-05 18:07:40.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/local.py
--rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-26 18:59:50.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/glue.py
--rw-r--r--   0 jwills     (501) staff       (20)     8611 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.592344 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 jwills     (501) staff       (20)     1291 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)      589 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 jwills     (501) staff       (20)     1669 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 jwills     (501) staff       (20)     1034 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 jwills     (501) staff       (20)     2050 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 jwills     (501) staff       (20)     1247 2023-05-05 18:05:09.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.592500 dbt-duckdb-1.5.1/dbt/include/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.592837 dbt-duckdb-1.5.1/dbt/include/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.593757 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/
--rw-r--r--   0 jwills     (501) staff       (20)     8151 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 jwills     (501) staff       (20)      950 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/catalog.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.594633 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 jwills     (501) staff       (20)     3916 2023-03-30 16:27:45.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1417 2023-04-03 22:00:10.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 jwills     (501) staff       (20)      792 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/snapshot_merge.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.596771 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/upstream.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.598343 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)    13064 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1615 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       60 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        4 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-05 18:27:10.599029 dbt-duckdb-1.5.1/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1366 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.680233 dbt-duckdb-1.5.2/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)    20476 2023-06-22 16:53:39.680080 dbt-duckdb-1.5.2/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)    20172 2023-06-22 16:52:09.000000 dbt-duckdb-1.5.2/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.671136 dbt-duckdb-1.5.2/dbt/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.671374 dbt-duckdb-1.5.2/dbt/adapters/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/adapters/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.673392 dbt-duckdb-1.5.2/dbt/adapters/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       18 2023-06-22 16:14:09.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3573 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7027 2023-06-17 00:24:18.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.674112 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 jwills     (501) staff       (20)     5307 2023-06-12 21:38:22.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2399 2023-06-12 21:38:22.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4923 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 jwills     (501) staff       (20)     8792 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.675505 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 jwills     (501) staff       (20)     4014 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)      489 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 jwills     (501) staff       (20)     8530 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/glue.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1666 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1029 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 jwills     (501) staff       (20)      533 2023-06-19 18:11:47.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/pd_utils.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1457 2023-06-19 18:11:47.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2519 2023-06-21 13:23:49.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2213 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.675672 dbt-duckdb-1.5.2/dbt/include/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.675922 dbt-duckdb-1.5.2/dbt/include/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.677340 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/
+-rw-r--r--   0 jwills     (501) staff       (20)     7996 2023-06-12 18:31:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      950 2023-05-05 22:17:51.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/catalog.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      643 2023-06-12 18:31:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/columns.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1429 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/incremental_helper.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.677911 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 jwills     (501) staff       (20)     4128 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     4679 2023-06-12 18:31:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1755 2023-06-07 23:05:13.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1359 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/snapshot_helper.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.679323 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/upstream.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.679936 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)    20476 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1751 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       60 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        4 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-06-22 16:53:39.680261 dbt-duckdb-1.5.2/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1366 2023-05-10 21:35:29.000000 dbt-duckdb-1.5.2/setup.py
```

### Comparing `dbt-duckdb-1.5.1/LICENSE` & `dbt-duckdb-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/connections.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/connections.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import atexit
 import threading
 from contextlib import contextmanager
+from typing import Tuple
+
+import agate
 
 import dbt.exceptions
 from . import environments
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterRequiredConfig
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.connection import Connection
@@ -15,14 +18,15 @@
 class DuckDBConnectionManager(SQLConnectionManager):
     TYPE = "duckdb"
     _LOCK = threading.RLock()
     _ENV = None
 
     def __init__(self, profile: AdapterRequiredConfig):
         super().__init__(profile)
+        self.disable_transactions = profile.credentials.disable_transactions  # type: ignore
 
     @classmethod
     def env(cls) -> environments.Environment:
         with cls._LOCK:
             if not cls._ENV:
                 raise Exception("DuckDBConnectionManager environment requested before creation!")
             return cls._ENV
@@ -86,9 +90,16 @@
 
     @classmethod
     def close_all_connections(cls):
         with cls._LOCK:
             if cls._ENV is not None:
                 cls._ENV = None
 
+    def execute(
+        self, sql: str, auto_begin: bool = False, fetch: bool = False, **kwargs
+    ) -> Tuple[AdapterResponse, agate.Table]:
+        if self.disable_transactions:
+            auto_begin = False
+        return super().execute(sql, auto_begin, fetch, **kwargs)
+
 
 atexit.register(DuckDBConnectionManager.close_all_connections)
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/credentials.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,21 +43,17 @@
             joined = ", ".join(options)
             base += f" ({joined})"
         return base
 
 
 @dataclass
 class PluginConfig(dbtClassMixin):
-    # The name that this plugin will be referred to by in sources/models; must
-    # be unique within the project
-    name: str
-
-    # The fully-specified class name of the plugin code to use, which must be a
-    # subclass of dbt.adapters.duckdb.plugins.Plugin.
-    impl: str
+    module: str
+
+    alias: Optional[str] = None
 
     # A plugin-specific set of configuration options
     config: Optional[Dict[str, Any]] = None
 
 
 @dataclass
 class Remote(dbtClassMixin):
@@ -112,14 +108,19 @@
     remote: Optional[Remote] = None
 
     # A list of dbt-duckdb plugins that can be used to customize the
     # behavior of loading source data and/or storing the relations that are
     # created by SQL or Python models; see the plugins module for more details.
     plugins: Optional[List[PluginConfig]] = None
 
+    # Whether to disable transactions when executing SQL statements; this
+    # is useful when we would like the resulting DuckDB database file to
+    # be as small as possible.
+    disable_transactions: bool = False
+
     @classmethod
     def __pre_deserialize__(cls, data: Dict[Any, Any]) -> Dict[Any, Any]:
         if duckdb.__version__ >= "0.7.0":
             data = super().__pre_deserialize__(data)
             if "database" not in data:
                 # if no database is specified in the profile, figure out
                 # the database value to use from the path argument
@@ -133,14 +134,19 @@
                     if db:
                         data["database"] = db
                     else:
                         raise dbt.exceptions.DbtRuntimeError(
                             "Unable to determine database name from path"
                             " and no database was specified in profile"
                         )
+                    # For MotherDuck, turn on disable_transactions unless
+                    # it's explicitly set already by the user
+                    if parsed.scheme in {"md", "motherduck"}:
+                        if "disable_transactions" not in data:
+                            data["disable_transactions"] = True
         return data
 
     @property
     def unique_field(self) -> str:
         if self.remote:
             return self.remote.host + str(self.remote.port)
         else:
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/__init__.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import abc
 import importlib.util
 import os
 import tempfile
 from typing import Dict
+from typing import Optional
 
 import duckdb
 
 from ..credentials import DuckDBCredentials
-from ..plugins import Plugin
+from ..plugins import BasePlugin
 from ..utils import SourceConfig
+from ..utils import TargetConfig
 from dbt.contracts.connection import AdapterResponse
 from dbt.exceptions import DbtRuntimeError
 
 
 def _ensure_event_loop():
     """
     Ensures the current thread has an event loop defined, and creates one if necessary.
@@ -42,26 +44,33 @@
     def submit_python_job(self, handle, parsed_model: dict, compiled_code: str) -> AdapterResponse:
         pass
 
     @abc.abstractmethod
     def load_source(self, plugin_name: str, source_config: SourceConfig) -> str:
         pass
 
+    @abc.abstractmethod
+    def store_relation(self, plugin_name: str, target_config: TargetConfig) -> None:
+        pass
+
     def get_binding_char(self) -> str:
         return "?"
 
     @classmethod
-    def initialize_db(cls, creds: DuckDBCredentials):
+    def initialize_db(
+        cls, creds: DuckDBCredentials, plugins: Optional[Dict[str, BasePlugin]] = None
+    ):
         config = creds.config_options or {}
         conn = duckdb.connect(creds.path, read_only=False, config=config)
 
         # install any extensions on the connection
         if creds.extensions is not None:
             for extension in creds.extensions:
-                conn.execute(f"INSTALL '{extension}'")
+                conn.install_extension(extension)
+                conn.load_extension(extension)
 
         # Attach any fsspec filesystems on the database
         if creds.filesystems:
             import fsspec
 
             for spec in creds.filesystems:
                 curr = spec.copy()
@@ -69,40 +78,40 @@
                 fs = fsspec.filesystem(fsimpl, **curr)
                 conn.register_filesystem(fs)
 
         # attach any databases that we will be using
         if creds.attach:
             for attachment in creds.attach:
                 conn.execute(attachment.to_sql())
+
+        # let the plugins do any configuration on the
+        # connection that they need to do
+        if plugins:
+            for plugin in plugins.values():
+                plugin.configure_connection(conn)
+
         return conn
 
     @classmethod
     def initialize_cursor(cls, creds: DuckDBCredentials, cursor):
-        # Extensions/settings need to be configured per cursor
-        for ext in creds.extensions or []:
-            cursor.execute(f"LOAD '{ext}'")
         for key, value in creds.load_settings().items():
             # Okay to set these as strings because DuckDB will cast them
             # to the correct type
             cursor.execute(f"SET {key} = '{value}'")
         return cursor
 
     @classmethod
-    def initialize_plugins(cls, creds: DuckDBCredentials) -> Dict[str, Plugin]:
+    def initialize_plugins(cls, creds: DuckDBCredentials) -> Dict[str, BasePlugin]:
         ret = {}
-        for plugin in creds.plugins or []:
-            if plugin.name in ret:
-                raise Exception("Duplicate plugin name: " + plugin.name)
-            else:
-                if plugin.impl in Plugin.WELL_KNOWN_PLUGINS:
-                    plugin.impl = Plugin.WELL_KNOWN_PLUGINS[plugin.impl]
-                try:
-                    ret[plugin.name] = Plugin.create(plugin.impl, plugin.config or {})
-                except Exception as e:
-                    raise Exception(f"Error attempting to create plugin {plugin.name}", e)
+        base_config = creds.settings or {}
+        for plugin_def in creds.plugins or []:
+            config = base_config.copy()
+            config.update(plugin_def.config or {})
+            plugin = BasePlugin.create(plugin_def.module, config=config, alias=plugin_def.alias)
+            ret[plugin.name] = plugin
         return ret
 
     @classmethod
     def run_python_job(cls, con, load_df_function, identifier: str, compiled_code: str):
         mod_file = tempfile.NamedTemporaryFile(suffix=".py", delete=False)
         mod_file.write(compiled_code.lstrip().encode("utf-8"))
         mod_file.close()
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/buenavista.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     @classmethod
     def _get_conn(cls, dbname: str, remote: credentials.Remote):
         return psycopg2.connect(
             dbname=dbname,
             user=remote.user,
             host=remote.host,
             port=remote.port,
+            password=remote.password,
         )
 
     def __init__(self, credentials: credentials.DuckDBCredentials):
         self.creds = credentials
         if not self.creds.remote:
             raise Exception("BVConnection only works with a remote host")
 
@@ -55,7 +56,21 @@
                 "source_config": source_config.as_dict(),
             },
         }
         cursor = handle.cursor()
         cursor.execute(json.dumps(payload))
         cursor.close()
         handle.close()
+
+    def store_relation(self, plugin_name: str, target_config: utils.TargetConfig) -> None:
+        handle = self.handle()
+        payload = {
+            "method": "dbt_store_relation",
+            "params": {
+                "plugin_name": plugin_name,
+                "target_config": target_config.as_dict(),
+            },
+        }
+        cursor = handle.cursor()
+        cursor.execute(json.dumps(payload))
+        cursor.close()
+        handle.close()
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/local.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/local.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,26 +43,31 @@
         # Set the conn attribute to None so it always exists even if
         # DB initialization fails
         self.conn = None
         self._plugins = self.initialize_plugins(credentials)
         self.creds = credentials
         self.handle_count = 0
         self.lock = threading.RLock()
+        self._keep_open = (
+            self.creds.path == ":memory:"
+            or self.creds.path.startswith("md:")
+            or self.creds.path.startswith("motherduck:")
+        )
 
     def notify_closed(self):
         with self.lock:
             self.handle_count -= 1
-            if self.handle_count == 0 and self.creds.path != ":memory:":
+            if self.handle_count == 0 and not self._keep_open:
                 self.close()
 
     def handle(self):
         # Extensions/settings need to be configured per cursor
         with self.lock:
             if self.conn is None:
-                self.conn = self.initialize_db(self.creds)
+                self.conn = self.initialize_db(self.creds, self._plugins)
             self.handle_count += 1
         cursor = self.initialize_cursor(self.creds, self.conn.cursor())
         return DuckDBConnectionWrapper(cursor, self)
 
     def submit_python_job(self, handle, parsed_model: dict, compiled_code: str) -> AdapterResponse:
         con = handle.cursor()
 
@@ -77,37 +82,57 @@
             raise Exception(
                 f"Plugin {plugin_name} not found; known plugins are: "
                 + ",".join(self._plugins.keys())
             )
         plugin = self._plugins[plugin_name]
         handle = self.handle()
         cursor = handle.cursor()
-        save_mode = source_config.meta.get("save_mode", "overwrite")
+        save_mode = source_config.get("save_mode", "overwrite")
         if save_mode in ("ignore", "error_if_exists"):
-            schema, identifier = source_config.schema, source_config.identifier
-            q = f"""SELECT COUNT(1)
-                FROM information_schema.tables
-                WHERE table_schema = '{schema}'
-                AND table_name = '{identifier}'
+            params = [source_config.schema, source_config.identifier]
+            q = """SELECT COUNT(1)
+                FROM system.information_schema.tables
+                WHERE table_schema = ?
+                AND table_name = ?
                 """
-            if cursor.execute(q).fetchone()[0]:
+            if source_config.database:
+                q += "AND table_catalog = ?"
+                params.append(source_config.database)
+            if cursor.execute(q, params).fetchone()[0]:
                 if save_mode == "error_if_exists":
                     raise Exception(f"Source {source_config.table_name()} already exists!")
                 else:
                     # Nothing to do (we ignore the existing table)
                     return
         df = plugin.load(source_config)
         assert df is not None
         materialization = source_config.meta.get("materialization", "table")
         cursor.execute(
             f"CREATE OR REPLACE {materialization} {source_config.table_name()} AS SELECT * FROM df"
         )
         cursor.close()
         handle.close()
 
+    def store_relation(self, plugin_name: str, target_config: utils.TargetConfig) -> None:
+        if plugin_name not in self._plugins:
+            if plugin_name.startswith("glue|"):
+                from ..plugins import glue
+
+                _, glue_db = plugin_name.split("|")
+                config = (self.creds.settings or {}).copy()
+                config["glue_database"] = glue_db
+                self._plugins[plugin_name] = glue.Plugin(plugin_name, config)
+            else:
+                raise Exception(
+                    f"Plugin {plugin_name} not found; known plugins are: "
+                    + ",".join(self._plugins.keys())
+                )
+        plugin = self._plugins[plugin_name]
+        plugin.store(target_config)
+
     def close(self):
         if self.conn:
             self.conn.close()
             self.conn = None
 
     def __del__(self):
         self.close()
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/glue.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/glue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Sequence
-from typing import Union
 
-from dbt.adapters.base.column import Column
-
-BOTO3_EXISTS = False
-
-try:
-    import boto3
-    from mypy_boto3_glue import GlueClient
-    from mypy_boto3_glue.type_defs import (
-        ColumnTypeDef,
-        GetTableResponseTypeDef,
-        SerDeInfoTypeDef,
-        StorageDescriptorTypeDef,
-        TableInputTypeDef,
-    )
+import boto3
+from mypy_boto3_glue import GlueClient
+from mypy_boto3_glue.type_defs import ColumnTypeDef
+from mypy_boto3_glue.type_defs import GetTableResponseTypeDef
+from mypy_boto3_glue.type_defs import SerDeInfoTypeDef
+from mypy_boto3_glue.type_defs import StorageDescriptorTypeDef
+from mypy_boto3_glue.type_defs import TableInputTypeDef
 
-    BOTO3_EXISTS = True
-except ImportError:
-    pass
+from . import BasePlugin
+from ..utils import TargetConfig
+from dbt.adapters.base.column import Column
 
 
 class UnsupportedFormatType(Exception):
     """UnsupportedFormatType exception."""
 
 
 class UnsupportedType(Exception):
@@ -164,66 +156,85 @@
 
 
 def _get_table_def(
     table: str,
     s3_path: str,
     columns: Sequence["ColumnTypeDef"],
     file_format: str,
-    **kwargs,
+    delimiter: str,
 ):
     s3_parent = "/".join(s3_path.split("/")[:-1])
     if file_format == "csv":
         table_def = _get_csv_table_def(
             table=table,
             s3_parent=s3_parent,
             columns=columns,
-            delimiter=kwargs.get("delimiter", ","),
+            delimiter=delimiter,
         )
     elif file_format == "parquet":
         table_def = _get_parquet_table_def(table=table, s3_parent=s3_parent, columns=columns)
     else:
         raise UnsupportedFormatType("Format %s is not supported in Glue registrar." % file_format)
     return table_def
 
 
-def _get_glue_client(settings: Optional[Dict[str, Any]]) -> "GlueClient":
+def _get_glue_client(settings: Dict[str, Any]) -> "GlueClient":
     if settings:
         return boto3.client(
             "glue",
             aws_access_key_id=settings.get("s3_access_key_id"),
             aws_secret_access_key=settings.get("s3_secret_access_key"),
             aws_session_token=settings.get("s3_session_token"),
             region_name=settings.get("s3_region"),
         )
     else:
         return boto3.client("glue")
 
 
 def create_or_update_table(
+    client: GlueClient,
     database: str,
     table: str,
     column_list: Sequence[Column],
     s3_path: str,
     file_format: str,
-    settings: Optional[Dict[str, Any]],
-    **kwargs: Optional[Dict[str, Union[str, int]]],
+    delimiter: str,
 ) -> None:
-    if BOTO3_EXISTS:
-        client = _get_glue_client(settings)
-        # Existing table in AWS Glue catalog
-        glue_table = _get_table(client=client, database=database, table=table)
-        columns = _convert_columns(column_list)
-        table_def = _get_table_def(
-            table=table,
-            s3_path=s3_path,
-            columns=columns,
-            file_format=file_format,
-            **kwargs,
+    # Existing table in AWS Glue catalog
+    glue_table = _get_table(client=client, database=database, table=table)
+    columns = _convert_columns(column_list)
+    table_def = _get_table_def(
+        table=table,
+        s3_path=s3_path,
+        columns=columns,
+        file_format=file_format,
+        delimiter=delimiter,
+    )
+    if glue_table:
+        # Existing columns in AWS Glue catalog
+        glue_columns = _get_column_type_def(glue_table)
+        # Create new version only if columns are changed
+        if glue_columns != columns:
+            _update_table(client=client, database=database, table_def=table_def)
+    else:
+        _create_table(client=client, database=database, table_def=table_def)
+
+
+class Plugin(BasePlugin):
+    def initialize(self, config: Dict[str, Any]):
+        self.client = _get_glue_client(config)
+        self.database = config.get("glue_database", "default")
+        self.delimiter = config.get("delimiter", ",")
+
+    def store(self, target_config: TargetConfig):
+        assert target_config.location is not None
+        assert target_config.relation.identifier is not None
+        table: str = target_config.relation.identifier
+        create_or_update_table(
+            self.client,
+            self.database,
+            table,
+            target_config.column_list,
+            target_config.location.path,
+            target_config.location.format,
+            self.delimiter,
         )
-        if glue_table:
-            # Existing columns in AWS Glue catalog
-            glue_columns = _get_column_type_def(glue_table)
-            # Create new version only if columns are changed
-            if glue_columns != columns:
-                _update_table(client=client, database=database, table_def=table_def)
-        else:
-            _create_table(client=client, database=database, table_def=table_def)
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/impl.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import duckdb
 
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.base.column import Column
 from dbt.adapters.base.impl import ConstraintSupport
 from dbt.adapters.base.meta import available
 from dbt.adapters.duckdb.connections import DuckDBConnectionManager
-from dbt.adapters.duckdb.glue import create_or_update_table
 from dbt.adapters.duckdb.relation import DuckDBRelation
+from dbt.adapters.duckdb.utils import TargetConfig
+from dbt.adapters.duckdb.utils import TargetLocation
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.nodes import ColumnLevelConstraint
 from dbt.contracts.graph.nodes import ConstraintType
 from dbt.exceptions import DbtInternalError
 from dbt.exceptions import DbtRuntimeError
 
@@ -53,42 +54,44 @@
                         )
                     ],
                     replace=True,
                 )
         return table
 
     @available
+    def get_seed_file_path(self, model) -> str:
+        return os.path.join(model["root_path"], model["original_file_path"])
+
+    @available
     def location_exists(self, location: str) -> bool:
         try:
             self.execute(
                 f"select 1 from '{location}' where 1=0",
                 auto_begin=False,
                 fetch=False,
             )
             return True
         except DbtRuntimeError:
             return False
 
     @available
-    def register_glue_table(
+    def store_relation(
         self,
-        glue_database: str,
-        table: str,
+        plugin_name: str,
+        relation: DuckDBRelation,
         column_list: Sequence[Column],
-        location: str,
-        file_format: str,
+        path: str,
+        format: str,
     ) -> None:
-        create_or_update_table(
-            database=glue_database,
-            table=table,
+        target_config = TargetConfig(
+            relation=relation,
             column_list=column_list,
-            s3_path=location,
-            file_format=file_format,
-            settings=self.config.credentials.settings,
+            location=TargetLocation(path=path, format=format),
         )
+        DuckDBConnectionManager.env().store_relation(plugin_name, target_config)
 
     @available
     def external_root(self) -> str:
         return self.config.credentials.external_root
 
     @available
     def use_database(self) -> bool:
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dataclasses import dataclass
+from typing import Any
 from typing import Dict
 from typing import Literal
 
 import gspread
 import pandas as pd
 
-from . import Plugin
+from . import BasePlugin
 from . import PluginConfig
 from ..utils import SourceConfig
 
 
 @dataclass
 class GSheetConfig(PluginConfig):
     method: Literal["service", "oauth"]
@@ -17,33 +18,33 @@
     def client(self):
         if self.method == "service":
             return gspread.service_account()
         else:
             return gspread.oauth()
 
 
-class GSheetPlugin(Plugin):
-    def __init__(self, config: Dict):
+class Plugin(BasePlugin):
+    def initialize(self, config: Dict[str, Any]):
         self._config = GSheetConfig.from_dict(config)
         self._gc = self._config.client()
 
     def load(self, source_config: SourceConfig):
         doc = None
-        if "title" in source_config.meta:
-            doc = self._gc.open(source_config.meta["title"])
-        elif "key" in source_config.meta:
-            doc = self._gc.open_by_key(source_config.meta["key"])
-        elif "url" in source_config.meta:
-            doc = self._gc.open_by_url(source_config.meta["url"])
+        if "title" in source_config:
+            doc = self._gc.open(source_config["title"])
+        elif "key" in source_config:
+            doc = self._gc.open_by_key(source_config["key"])
+        elif "url" in source_config:
+            doc = self._gc.open_by_url(source_config["url"])
         else:
             raise Exception("Source config did not indicate a method to open a GSheet to read")
 
         sheet = None
-        if "worksheet" in source_config.meta:
-            work_id = source_config.meta["worksheet"]
+        if "worksheet" in source_config:
+            work_id = source_config["worksheet"]
             if isinstance(work_id, int):
                 sheet = doc.get_worksheet(work_id)
             elif isinstance(work_id, str):
                 sheet = doc.worksheet(work_id)
             else:
                 raise Exception(
                     f"Could not identify a worksheet in the doc from identifier: {work_id}"
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from typing import Any
 from typing import Dict
 
 import pyiceberg.catalog
 
-from . import Plugin
+from . import BasePlugin
 from ..utils import SourceConfig
 
 
-class IcebergPlugin(Plugin):
-    def __init__(self, config: Dict):
+class Plugin(BasePlugin):
+    def initialize(self, config: Dict[str, Any]):
         if "catalog" not in config:
             raise Exception("'catalog' is a required argument for the iceberg plugin!")
         catalog = config.pop("catalog")
         self._catalog = pyiceberg.catalog.load_catalog(catalog, **config)
 
     def load(self, source_config: SourceConfig):
-        table_format = source_config.meta.get("iceberg_table", "{schema}.{identifier}")
+        table_format = source_config.get("iceberg_table", "{schema}.{identifier}")
         table_name = table_format.format(**source_config.as_dict())
         table = self._catalog.load_table(table_name)
         scan_keys = {
             "row_filter",
             "selected_fields",
             "case_sensitive",
             "snapshot_id",
             "options",
             "limit",
         }
-        scan_config = {k: source_config.meta[k] for k in scan_keys if k in source_config.meta}
+        scan_config = {k: source_config[k] for k in scan_keys if k in source_config}
         return table.scan(**scan_config).to_arrow()
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 from typing import Any
 from typing import Dict
 
 import pandas as pd
 from sqlalchemy import create_engine
 from sqlalchemy import text
 
-from . import Plugin
+from . import BasePlugin
+from . import pd_utils
 from ..utils import SourceConfig
+from ..utils import TargetConfig
 
 
-class SQLAlchemyPlugin(Plugin):
-    def __init__(self, plugin_config: Dict[str, Any]):
+class Plugin(BasePlugin):
+    def initialize(self, plugin_config: Dict[str, Any]):
         self.engine = create_engine(plugin_config["connection_url"])
 
     def load(self, source_config: SourceConfig) -> pd.DataFrame:
-        if "query" in source_config.meta:
-            query = source_config.meta["query"]
+        if "query" in source_config:
+            query = source_config["query"]
             query = query.format(**source_config.as_dict())
-            params = source_config.meta.get("params", {})
+            params = source_config.get("params", {})
             with self.engine.connect() as conn:
                 return pd.read_sql_query(text(query), con=conn, params=params)
         else:
-            if "table" in source_config.meta:
-                table = source_config.meta["table"]
+            if "table" in source_config:
+                table = source_config["table"]
             else:
                 table = source_config.table_name()
             with self.engine.connect() as conn:
                 return pd.read_sql_table(table, con=conn)
+
+    def store(self, target_config: TargetConfig):
+        # first, load the data frame from the external location
+        df = pd_utils.target_to_df(target_config)
+        table_name = target_config.relation.identifier
+        # then, write it to the database
+        df.to_sql(table_name, self.engine, if_exists="replace", index=False)
+
+    def __del__(self):
+        self.engine.dispose()
```

### Comparing `dbt-duckdb-1.5.1/dbt/adapters/duckdb/relation.py` & `dbt-duckdb-1.5.2/dbt/adapters/duckdb/relation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from string import Template
 from typing import Any
 from typing import Optional
 from typing import Type
 
 from .connections import DuckDBConnectionManager
 from .utils import SourceConfig
 from dbt.adapters.base.relation import BaseRelation
@@ -12,30 +13,38 @@
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DuckDBRelation(BaseRelation):
     external: Optional[str] = None
 
     @classmethod
     def create_from_source(cls: Type[Self], source: SourceDefinition, **kwargs: Any) -> Self:
-        source_config = SourceConfig.create(source)
+        source_config = SourceConfig.create_from_source(source)
         # First check to see if a 'plugin' is defined in the meta argument for
         # the source or its parent configuration, and if it is, use the environment
         # associated with this run to get the name of the source that we should
         # reference in the compiled model
-        if "plugin" in source_config.meta:
-            plugin_name = source_config.meta["plugin"]
-            DuckDBConnectionManager.env().load_source(plugin_name, source_config)
-        elif "external_location" in source_config.meta:
-            # Call str.format with the schema, name and identifier for the source so that they
-            # can be injected into the string; this helps reduce boilerplate when all
-            # of the tables in the source have a similar location based on their name
-            # and/or identifier.
-            ext_location = source_config.meta["external_location"].format(
-                **source_config.as_dict()
-            )
+        if "plugin" in source_config:
+            plugin_name = source_config["plugin"]
+            if DuckDBConnectionManager._ENV is not None:
+                # No connection means we are probably in the dbt parsing phase, so don't load yet.
+                DuckDBConnectionManager.env().load_source(plugin_name, source_config)
+        elif "external_location" in source_config:
+            ext_location_template = source_config["external_location"]
+            formatter = source_config.get("formatter", "newstyle")
+            if formatter == "newstyle":
+                ext_location = ext_location_template.format_map(source_config.as_dict())
+            elif formatter == "oldstyle":
+                ext_location = ext_location_template % source_config.as_dict()
+            elif formatter == "template":
+                ext_location = Template(ext_location_template).substitute(source_config.as_dict())
+            else:
+                raise ValueError(
+                    f"Formatter {formatter} not recognized. Must be one of 'newstyle', 'oldstyle', or 'template'."
+                )
+
             # If it's a function call or already has single quotes, don't add them
             if "(" not in ext_location and not ext_location.startswith("'"):
                 ext_location = f"'{ext_location}'"
             kwargs["external"] = ext_location
 
         return super().create_from_source(source, **kwargs)  # type: ignore
```

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/adapters.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/adapters.sql`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,30 @@
     drop schema if exists {{ relation.without_identifier().include(database=adapter.use_database()) }} cascade
   {%- endcall -%}
 {% endmacro %}
 
 {% macro duckdb__list_schemas(database) -%}
   {% set sql %}
     select schema_name
-    from information_schema.schemata
+    from system.information_schema.schemata
+    {% if database is not none %}
+    where catalog_name = '{{ database }}'
+    {% endif %}
   {% endset %}
   {{ return(run_query(sql)) }}
 {% endmacro %}
 
 {% macro duckdb__check_schema_exists(information_schema, schema) -%}
   {% set sql -%}
         select count(*)
-        from information_schema.schemata
-        where schema_name='{{ schema }}'
+        from system.information_schema.schemata
+        where schema_name = '{{ schema }}'
+        {% if adapter.use_database() %}
+        and catalog_name = '{{ information_schema.database }}'
+        {% endif %}
   {%- endset %}
   {{ return(run_query(sql)) }}
 {% endmacro %}
 
 {% macro get_column_names() %}
   {# loop through user_provided_columns to get column names #}
     {%- set user_provided_columns = model['columns'] -%}
@@ -104,19 +110,22 @@
       select
           column_name,
           data_type,
           character_maximum_length,
           numeric_precision,
           numeric_scale
 
-      from information_schema.columns
+      from system.information_schema.columns
       where table_name = '{{ relation.identifier }}'
-        {% if relation.schema %}
-        and table_schema = '{{ relation.schema }}'
-        {% endif %}
+      {% if relation.schema %}
+      and table_schema = '{{ relation.schema }}'
+      {% endif %}
+      {% if adapter.use_database() and relation.database %}
+      and table_catalog = '{{ relation.database }}'
+      {% endif %}
       order by ordinal_position
 
   {% endcall %}
   {% set table = load_result('get_columns_in_relation').table %}
   {{ return(sql_convert_columns_in_relation(table)) }}
 {% endmacro %}
 
@@ -127,16 +136,19 @@
       table_name as name,
       table_schema as schema,
       CASE table_type
         WHEN 'BASE TABLE' THEN 'table'
         WHEN 'VIEW' THEN 'view'
         WHEN 'LOCAL TEMPORARY' THEN 'table'
         END as type
-    from information_schema.tables
+    from system.information_schema.tables
     where table_schema = '{{ schema_relation.schema }}'
+    {% if adapter.use_database() %}
+    and table_catalog = '{{ schema_relation.database }}'
+    {% endif %}
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 {% macro duckdb__drop_relation(relation) -%}
   {% call statement('drop_relation', auto_begin=False) -%}
     drop {{ relation.type }} if exists {{ relation.include(database=adapter.use_database()) }} cascade
@@ -179,37 +191,27 @@
   {{ current_timestamp() }}::timestamp
 {%- endmacro %}
 
 {% macro duckdb__get_incremental_default_sql(arg_dict) %}
   {% do return(get_incremental_delete_insert_sql(arg_dict)) %}
 {% endmacro %}
 
-{% macro duckdb__get_incremental_delete_insert_sql(arg_dict) %}
-  {% do return(get_delete_insert_merge_sql(arg_dict["target_relation"].include(database=adapter.use_database()), arg_dict["temp_relation"], arg_dict["unique_key"], arg_dict["dest_columns"])) %}
-{% endmacro %}
-
-{% macro duckdb__get_incremental_append_sql(arg_dict) %}
-  {% do return(get_insert_into_sql(arg_dict["target_relation"].include(database=adapter.use_database()), arg_dict["temp_relation"], arg_dict["dest_columns"])) %}
-{% endmacro %}
-
 {% macro location_exists(location) -%}
   {% do return(adapter.location_exists(location)) %}
 {% endmacro %}
 
 {% macro write_to_file(relation, location, options) -%}
   {% call statement('write_to_file') -%}
     copy {{ relation }} to '{{ location }}' ({{ options }})
   {%- endcall %}
 {% endmacro %}
 
-{% macro register_glue_table(register, glue_database, relation, location, format) -%}
-  {% if location.startswith("s3://") and register == true %}
-    {%- set column_list = adapter.get_columns_in_relation(relation) -%}
-    {% do adapter.register_glue_table(glue_database, relation.identifier, column_list, location, format) %}
-  {% endif %}
+{% macro store_relation(plugin, relation, location, format) -%}
+  {%- set column_list = adapter.get_columns_in_relation(relation) -%}
+  {% do adapter.store_relation(plugin, relation, column_list, location, format) %}
 {% endmacro %}
 
 {% macro render_write_options(config) -%}
   {% set options = config.get('options', {}) %}
   {% for k in options %}
     {% if options[k] is string %}
       {% set _ = options.update({k: render(options[k])}) %}
```

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/catalog.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/external.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,22 @@
   {{ adapter.commit() }}
 
   -- finally, drop the existing/backup relation after the commit
   {{ drop_relation_if_exists(backup_relation) }}
   {{ drop_relation_if_exists(temp_relation) }}
 
   -- register table into glue
+  {%- set plugin_name = config.get('plugin') -%}
   {%- set glue_register = config.get('glue_register', default=false) -%}
-  {%- set glue_database = render(config.get('glue_database', default='default')) -%}
-  {% do register_glue_table(glue_register, glue_database, target_relation, location, format) %}
+  {% if plugin_name is not none or glue_register is true %}
+    {% if glue_register %}
+      {# legacy hack to set the glue database name, deprecate this #}
+      {%- set plugin_name = 'glue|' ~ config.get('glue_database', 'default') -%}
+    {% endif %}
+    {% do store_relation(plugin_name, target_relation, location, format) %}
+  {% endif %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
```

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     {% set dest_columns = process_schema_changes(on_schema_change, temp_relation, existing_relation) %}
     {% if not dest_columns %}
       {% set dest_columns = adapter.get_columns_in_relation(existing_relation) %}
     {% endif %}
 
     {#-- Get the incremental_strategy, the macro to use for the strategy, and build the sql --#}
     {% set incremental_strategy = config.get('incremental_strategy') or 'default' %}
-    {% set incremental_predicates = config.get('incremental_predicates', none) %}
+    {% set incremental_predicates = config.get('predicates', none) or config.get('incremental_predicates', none) %}
     {% set strategy_sql_macro_func = adapter.get_incremental_strategy_macro(context, incremental_strategy) %}
-    {% set strategy_arg_dict = ({'target_relation': target_relation, 'temp_relation': temp_relation, 'unique_key': unique_key, 'dest_columns': dest_columns, 'predicates': incremental_predicates }) %}
+    {% set strategy_arg_dict = ({'target_relation': target_relation, 'temp_relation': temp_relation, 'unique_key': unique_key, 'dest_columns': dest_columns, 'incremental_predicates': incremental_predicates }) %}
     {% set build_sql = strategy_sql_macro_func(strategy_arg_dict) %}
     {% set language = "sql" %}
 
   {% endif %}
 
   {% call statement("main", language=language) %}
       {{- build_sql }}
```

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/table.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/seed.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/seed.sql`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 {% endmacro %}
 
 {% macro duckdb__get_batch_size() %}
   {{ return(10000) }}
 {% endmacro %}
 
 {% macro duckdb__load_csv_rows(model, agate_table) %}
+    {% if config.get('fast') %}
+        {% set seed_file_path = adapter.get_seed_file_path(model) %}
+        {% set sql %}
+          COPY {{ this.render() }} FROM '{{ seed_file_path }}' (FORMAT CSV, HEADER TRUE)
+        {% endset %}
+        {% do adapter.add_query(sql, abridge_sql_log=True) %}
+        {{ return(sql) }}
+    {% endif %}
+
     {% set batch_size = get_batch_size() %}
     {% set agate_table = adapter.convert_datetimes_to_strs(agate_table) %}
     {% set cols_sql = get_seed_column_quoted_csv(model, agate_table.column_names) %}
     {% set bindings = [] %}
 
     {% set statements = [] %}
```

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/datediff.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.1/dbt_duckdb.egg-info/SOURCES.txt` & `dbt-duckdb-1.5.2/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 setup.py
 dbt/__init__.py
 dbt/adapters/__init__.py
 dbt/adapters/duckdb/__init__.py
 dbt/adapters/duckdb/__version__.py
 dbt/adapters/duckdb/connections.py
 dbt/adapters/duckdb/credentials.py
-dbt/adapters/duckdb/glue.py
 dbt/adapters/duckdb/impl.py
 dbt/adapters/duckdb/relation.py
 dbt/adapters/duckdb/utils.py
 dbt/adapters/duckdb/environments/__init__.py
 dbt/adapters/duckdb/environments/buenavista.py
 dbt/adapters/duckdb/environments/local.py
 dbt/adapters/duckdb/plugins/__init__.py
 dbt/adapters/duckdb/plugins/excel.py
+dbt/adapters/duckdb/plugins/glue.py
 dbt/adapters/duckdb/plugins/gsheet.py
 dbt/adapters/duckdb/plugins/iceberg.py
+dbt/adapters/duckdb/plugins/pd_utils.py
 dbt/adapters/duckdb/plugins/sqlalchemy.py
 dbt/include/__init__.py
 dbt/include/duckdb/__init__.py
 dbt/include/duckdb/dbt_project.yml
 dbt/include/duckdb/macros/adapters.sql
 dbt/include/duckdb/macros/catalog.sql
+dbt/include/duckdb/macros/columns.sql
+dbt/include/duckdb/macros/incremental_helper.sql
 dbt/include/duckdb/macros/seed.sql
-dbt/include/duckdb/macros/snapshot_merge.sql
+dbt/include/duckdb/macros/snapshot_helper.sql
 dbt/include/duckdb/macros/materializations/external.sql
 dbt/include/duckdb/macros/materializations/incremental.sql
 dbt/include/duckdb/macros/materializations/table.sql
 dbt/include/duckdb/macros/utils/any_value.sql
 dbt/include/duckdb/macros/utils/dateadd.sql
 dbt/include/duckdb/macros/utils/datediff.sql
 dbt/include/duckdb/macros/utils/external_location.sql
```

### Comparing `dbt-duckdb-1.5.1/setup.py` & `dbt-duckdb-1.5.2/setup.py`

 * *Files identical despite different names*

