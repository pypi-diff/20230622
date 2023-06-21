# Comparing `tmp/in-dbt-spark-1.2.521.tar.gz` & `tmp/in-dbt-spark-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.2.521.tar", last modified: Wed Jun 21 22:48:44 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.5.0.tar", last modified: Thu Jun  1 19:24:18 2023, max compression
```

## Comparing `in-dbt-spark-1.2.521.tar` & `in-dbt-spark-1.5.0.tar`

### file list

```diff
@@ -1,63 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.324857 in-dbt-spark-1.2.521/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-21 22:48:44.324857 in-dbt-spark-1.2.521/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.316856 in-dbt-spark-1.2.521/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.316856 in-dbt-spark-1.2.521/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.320857 in-dbt-spark-1.2.521/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.320857 in-dbt-spark-1.2.521/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    25291 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.316856 in-dbt-spark-1.2.521/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.320857 in-dbt-spark-1.2.521/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.320857 in-dbt-spark-1.2.521/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.320857 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.320857 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.324857 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:48:44.324857 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-21 22:48:44.000000 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-21 22:48:44.000000 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:48:44.000000 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:48:44.000000 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-21 22:48:44.000000 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 22:48:44.000000 in-dbt-spark-1.2.521/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:48:44.324857 in-dbt-spark-1.2.521/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-21 22:48:32.000000 in-dbt-spark-1.2.521/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.134134 in-dbt-spark-1.5.0/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.134134 in-dbt-spark-1.5.0/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25553 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25848 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.134134 in-dbt-spark-1.5.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.138134 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 19:24:18.000000 in-dbt-spark-1.5.0/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:24:18.142134 in-dbt-spark-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-01 19:24:06.000000 in-dbt-spark-1.5.0/setup.py
```

### Comparing `in-dbt-spark-1.2.521/PKG-INFO` & `in-dbt-spark-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.521
+Version: 1.5.0
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ODBC
 Provides-Extra: PyHive
 Provides-Extra: session
 Provides-Extra: all
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-spark/actions/workflows/main.yml">
     <img src="https://github.com/dbt-labs/dbt-spark/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
   </a>
-  <a href="https://github.com/dbt-labs/dbt-spark/actions/workflows/integration.yml">
-    <img src="https://github.com/dbt-labs/dbt-spark/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+  <a href="https://circleci.com/gh/dbt-labs/dbt-spark/?branch=main">
+    <img src="https://circleci.com/gh/dbt-labs/dbt-spark/tree/main.svg?style=shield" alt="Integration Tests Badge"/>
   </a>
 </p>
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.521 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.0 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: ODBC Provides-Extra: PyHive Provides-Extra: session Provides-
-Extra: all
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: ODBC
+Provides-Extra: PyHive Provides-Extra: session Provides-Extra: all
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## in-dbt-spark The `in-dbt-spark` package contains code to
```

### Comparing `in-dbt-spark-1.2.521/README.md` & `in-dbt-spark-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-spark/actions/workflows/main.yml">
     <img src="https://github.com/dbt-labs/dbt-spark/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
   </a>
-  <a href="https://github.com/dbt-labs/dbt-spark/actions/workflows/integration.yml">
-    <img src="https://github.com/dbt-labs/dbt-spark/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+  <a href="https://circleci.com/gh/dbt-labs/dbt-spark/?branch=main">
+    <img src="https://circleci.com/gh/dbt-labs/dbt-spark/tree/main.svg?style=shield" alt="Integration Tests Badge"/>
   </a>
 </p>
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/client.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/client.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/models.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def raise_for_status(self) -> None:
         if not self.execution_success:
             logger.error(f"Spark Runtime Error : {self.error}")
             components = []
             if self.error is not None:
                 components.append(f"Error ={self.error}")
-            raise dbt.exceptions.RuntimeException(f'({", ".join(components)})')
+            raise dbt.exceptions.DbtRuntimeError(f'({", ".join(components)})')
 
 
 class StatementKind(Enum):
     SPARK = "spark"
     PYSPARK = "pyspark"
     SPARKR = "sparkr"
     SQL = "sql"
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/session.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,25 +61,25 @@
             time.sleep(interval)
         if self.state in SESSION_INVALID_STATE:
             # Log setu submit error for dead state
             if self.state == SessionState.DEAD:
                 logger.error(self.client.get_log(self.session_id))
             logger.error(f"Unable to create setu session with {self.session_id} with error:")
             logger.error(self.diagnostics)
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f" Setu session state = {self.state} Unable to create setu session with {self.session_id}"
             )
         self.print_session_details()
 
     @property
     def state(self) -> SessionState:
         """The state of the managed SETU session."""
         session = self.client.get_session(self.session_id)
         if session is None:
-            raise dbt.exceptions.RuntimeException("session not found - it may have been shut down")
+            raise dbt.exceptions.DbtRuntimeError("session not found - it may have been shut down")
 
         if session.state in SESSION_INVALID_STATE:
             self.diagnostics = session.diagnostics
         return session.state
 
     def cursor(self) -> SetuStatementCursor:
         """create new SETU statement"""
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/session_cursor.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,30 +60,30 @@
             )
             time.sleep(next(intervals))
             self.statement = self.client.get_statement(
                 self.statement.session_id, self.statement.statement_id
             )
         if self.statement.output is None:
             logger.error(f" Setu Statement {self.statement.statement_id} had no output ")
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"Setu Statement {self.statement.statement_id} had no output"
             )
         logger.info(
             "Setu Statement {} state is : {}".format(
                 self.statement.statement_id, self.statement.state
             )
         )
         self.statement.output.raise_for_status()
         if not self.statement.output.execution_success:
             logger.error(
                 "Setu Statement {} output Error : {}".format(
                     self.statement.statement_id, self.statement.output
                 )
             )
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"Error during Setu Statement {self.statement.statement_id} execution : {self.statement.output.error}"
             )
         return self.statement.output
 
     def close(self):
         if self.statement is not None and self.statement.state in [
             StatementState.WAITING,
@@ -112,29 +112,29 @@
                 )
                 time.sleep(next(intervals))
                 self.statement = self.client.get_statement(
                     self.statement.session_id, self.statement.statement_id
                 )
             if self.statement.output is None:
                 logger.error(f"Setu Statement {self.statement.statement_id} had no output")
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f"Setu Statement {self.statement.statement_id} had no output"
                 )
             self.statement.output.raise_for_status()
             if self.statement.output.json is None:
                 logger.error(f"Setu statement {self.statement.statement_id} had no JSON output")
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f"Setu statement {self.statement.statement_id} had no JSON output"
                 )
             return get_data_from_json_output(self.statement.output.json)
         elif self.statement is not None:
             self.statement.output.raise_for_status()
             return get_data_from_json_output(self.statement.output.json)
         else:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 "Setu statement response : {} ".format(self.statement)
             )
 
     def get_formatted_code(self, code: str) -> str:
         code_lines = []
         for line in code.splitlines():
             line = line.strip()
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/session_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         :param metadata: Dict of metadata for this SETU session
         :param enable_ssl: enable ssl configurations on driver and executors
         :param execution_tags: Dict of tags to be inferred by Infra
         :param spark_version: version of the spark session
         :param manifest_file_location: location of manifest file with all the dependencies
         """
         with cls.session_lock:
-
             session_initialization_config = SessionInitializationConfig(
                 proxy_user=proxy_user,
                 jars=jars,
                 py_files=py_files,
                 files=files,
                 archives=archives,
                 manifest_file_location=manifest_file_location,
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.5.0/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/spark/column.py` & `in-dbt-spark-1.5.0/dbt/adapters/spark/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from dbt.dataclass_schema import dbtClassMixin
 from hologram import JsonDict
 
 Self = TypeVar("Self", bound="SparkColumn")
 
 
 @dataclass
-class SparkColumn(dbtClassMixin, Column):
+class SparkColumn(dbtClassMixin, Column):  # type: ignore
     table_database: Optional[str] = None
     table_schema: Optional[str] = None
     table_name: Optional[str] = None
     table_type: Optional[str] = None
     table_owner: Optional[str] = None
     table_stats: Optional[Dict[str, Any]] = None
     column_index: Optional[int] = None
 
     @classmethod
     def translate_type(cls, dtype: str) -> str:
         return dtype
 
-    def can_expand_to(self: Self, other_column: Self) -> bool:
+    def can_expand_to(self: Self, other_column: Self) -> bool:  # type: ignore
         """returns True if both columns are strings"""
         return self.is_string() and other_column.is_string()
 
     def literal(self, value):
         return "cast({} as {})".format(value, self.dtype)
 
     @property
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.5.0/dbt/adapters/spark/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 from dbt.events import AdapterLogger
 from dbt.utils import DECIMALS
 from dbt.adapters.setu.session_manager import SetuSessionManager, SetuCluster
 from dbt.adapters.setu.session_handler import SetuSessionHandler
 from dbt.adapters.setu.constants import DEFAULT_HEARTBEAT_TIMEOUT
 from dbt.adapters.spark import __version__
 
-from dbt.adapters.setu.constants import Platform
-from dbt.adapters.setu.utils import get_platform
-
 try:
     from TCLIService.ttypes import TOperationState as ThriftState
     from thrift.transport import THttpClient
     from pyhive import hive
 except ImportError:
     ThriftState = None
     THttpClient = None
@@ -27,15 +24,15 @@
 except ImportError:
     pyodbc = None
 from datetime import datetime
 import sqlparams
 
 from hologram.helpers import StrEnum
 from dataclasses import dataclass, field
-from typing import Any, Dict, Optional, List
+from typing import Any, Dict, Optional, Union, List
 
 try:
     from thrift.transport.TSSLSocket import TSSLSocket
     import thrift
     import ssl
     import sasl
     import thrift_sasl
@@ -70,14 +67,15 @@
     host: Optional[str] = None
     database: Optional[str] = None
     driver: Optional[str] = None
     cluster: Optional[str] = None
     endpoint: Optional[str] = None
     token: Optional[str] = None
     user: Optional[str] = None
+    password: Optional[str] = None
     port: int = 443
     auth: Optional[str] = None
     kerberos_service_name: Optional[str] = None
 
     #  **********   setu specific configs   **********
     url: Optional[str] = None
     session_name: Optional[str] = None
@@ -110,86 +108,81 @@
     @classmethod
     def __pre_deserialize__(cls, data):
         data = super().__pre_deserialize__(data)
         if "database" not in data:
             data["database"] = None
         # since we write OpenHouse tables by default,
         # if 'schema' is defined but not in the expected 'openhouse.schema' format, prefix this automatically for the user
-        # if platform is darwin, don't enforce openhouse (since preview doesn't support trino right now)
-        if (
-            "schema" in data
-            and "." not in data["schema"]
-            and get_platform() != Platform.DARWIN_PLATFORM
-        ):
+        if "schema" in data and "." not in data["schema"]:
             data["schema"] = DEFAULT_CATALOG + "." + data["schema"]
         return data
 
+    @property
+    def cluster_id(self):
+        return self.cluster
+
     def __post_init__(self):
         if self.method == SparkConnectionMethod.ODBC:
             try:
                 import pyodbc  # noqa: F401
             except ImportError as e:
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f"{self.method} connection method requires "
                     "additional dependencies. \n"
                     "Install the additional required dependencies with "
                     "`pip install dbt-spark[ODBC]`\n\n"  # TODO: reword remedy here as we are in-dbt-spark
                     f"ImportError({e.msg})"
                 ) from e
 
         if self.method == SparkConnectionMethod.ODBC and self.cluster and self.endpoint:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 "`cluster` and `endpoint` cannot both be set when"
                 f" using {self.method} method to connect to Spark"
             )
 
         if (
             self.method == SparkConnectionMethod.HTTP
             or self.method == SparkConnectionMethod.THRIFT
         ) and not (ThriftState and THttpClient and hive):
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"{self.method} connection method requires "
                 "additional dependencies. \n"
                 "Install the additional required dependencies with "
                 "`pip install dbt-spark[PyHive]`"  # TODO: reword remedy here as we are in-dbt-spark
             )
 
         if self.method == SparkConnectionMethod.SESSION:
             try:
                 import pyspark  # noqa: F401
             except ImportError as e:
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f"{self.method} connection method requires "
                     "additional dependencies. \n"
                     "Install the additional required dependencies with "
                     "`pip install dbt-spark[session]`\n\n"  # TODO: reword remedy here as we are in-dbt-spark
                     f"ImportError({e.msg})"
                 ) from e
 
         if self.method == SparkConnectionMethod.SETU and (
             self.schema is None or self.session_name is None or self.proxy_user is None
         ):
             logger.error(" `schema`, `session_name`, `proxy_user` must be set in profile config")
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 " `schema`, `session_name`, `proxy_user` must be set when"
                 f" using {self.method} method to connect to Spark"
             )
 
     @property
     def type(self):
         return "spark"
 
     @property
     def unique_field(self):
         if self.method == SparkConnectionMethod.SETU:
-            if not self.cluster:
-                raise dbt.exceptions.DbtRuntimeError(
-                    "`cluster` must be set when using the Setu method to connect to Spark"
-                )
-            return self.cluster
+            return self.url
         else:
             return self.host
 
     def _connection_keys(self):
         if self.method == SparkConnectionMethod.SETU:
             return ("url", "schema", "session_name")
         else:
@@ -274,20 +267,21 @@
         # cancelled, for instance. The errorMessage will be None, but the
         # state of the query will be "cancelled". By raising an exception
         # here, we prevent dbt from showing a status of OK when the query
         # has in fact failed.
         if poll_state.errorMessage:
             logger.debug("Poll response: {}".format(poll_state))
             logger.debug("Poll status: {}".format(state))
-            dbt.exceptions.raise_database_error(poll_state.errorMessage)
+            raise dbt.exceptions.DbtDatabaseError(poll_state.errorMessage)
 
         elif state not in STATE_SUCCESS:
             status_type = ThriftState._VALUES_TO_NAMES.get(state, "Unknown<{!r}>".format(state))
-
-            dbt.exceptions.raise_database_error("Query failed with status: {}".format(status_type))
+            raise dbt.exceptions.DbtDatabaseError(
+                "Query failed with status: {}".format(status_type)
+            )
 
         logger.debug("Poll status: {}, query complete".format(state))
 
     @classmethod
     def _fix_binding(cls, value):
         """Convert complex datatypes to primitives that can be loaded by
         the Spark driver"""
@@ -334,17 +328,17 @@
             logger.debug(exc)
             if len(exc.args) == 0:
                 raise
 
             thrift_resp = exc.args[0]
             if hasattr(thrift_resp, "status"):
                 msg = thrift_resp.status.errorMessage
-                raise dbt.exceptions.RuntimeException(msg)
+                raise dbt.exceptions.DbtRuntimeError(msg)
             else:
-                raise dbt.exceptions.RuntimeException(str(exc))
+                raise dbt.exceptions.DbtRuntimeError(str(exc))
 
     def cancel(self, connection):
         connection.handle.cancel()
 
     @classmethod
     def get_response(cls, cursor) -> AdapterResponse:
         # https://github.com/dbt-labs/dbt-spark/issues/142
@@ -428,23 +422,25 @@
                     if creds.use_ssl:
                         transport = build_ssl_transport(
                             host=creds.host,
                             port=creds.port,
                             username=creds.user,
                             auth=creds.auth,
                             kerberos_service_name=creds.kerberos_service_name,
+                            password=creds.password,
                         )
                         conn = hive.connect(thrift_transport=transport)
                     else:
                         conn = hive.connect(
                             host=creds.host,
                             port=creds.port,
                             username=creds.user,
                             auth=creds.auth,
                             kerberos_service_name=creds.kerberos_service_name,
+                            password=creds.password,
                         )  # noqa
                     handle = PyhiveConnectionWrapper(conn)
                 elif creds.method == SparkConnectionMethod.ODBC:
                     if creds.cluster is not None:
                         required_fields = [
                             "driver",
                             "host",
@@ -453,21 +449,15 @@
                             "organization",
                             "cluster",
                         ]
                         http_path = cls.SPARK_CLUSTER_HTTP_PATH.format(
                             organization=creds.organization, cluster=creds.cluster
                         )
                     elif creds.endpoint is not None:
-                        required_fields = [
-                            "driver",
-                            "host",
-                            "port",
-                            "token",
-                            "endpoint",
-                        ]
+                        required_fields = ["driver", "host", "port", "token", "endpoint"]
                         http_path = cls.SPARK_SQL_ENDPOINT_HTTP_PATH.format(
                             endpoint=creds.endpoint
                         )
                     else:
                         raise dbt.exceptions.DbtProfileError(
                             "Either `cluster` or `endpoint` must set when"
                             " using the odbc method to connect to Spark"
@@ -536,15 +526,15 @@
                         archives=creds.archives,
                         files=creds.files,
                         manifest_file_location=creds.manifest_file_location,
                         heartbeat_timeout_in_seconds=creds.heartbeat_timeout_in_seconds,
                     )
                     if setu_session.session_id is None:
                         logger.error("Error creating Setu session")
-                        raise dbt.exceptions.RuntimeException(
+                        raise dbt.exceptions.DbtRuntimeError(
                             f"Error creating Setu session : {setu_session}"
                         )
                     setu_session.wait_till_ready()
                     logger.info(f"Setu session {setu_session.session_id} creation complete")
                     handle = SetuSessionHandler(handle=setu_session)
                 else:
                     raise dbt.exceptions.DbtProfileError(
@@ -555,15 +545,15 @@
                 exc = e
                 if isinstance(e, EOFError):
                     # The user almost certainly has invalid credentials.
                     # Perhaps a token expired, or something
                     msg = "Failed to connect"
                     if creds.token is not None:
                         msg += ", is your token valid?"
-                    raise dbt.exceptions.FailedToConnectException(msg) from e
+                    raise dbt.exceptions.FailedToConnectError(msg) from e
                 retryable_message = _is_retryable_error(e)
                 if retryable_message and creds.connect_retries > 0:
                     msg = (
                         f"Warning: {retryable_message}\n\tRetrying in "
                         f"{creds.connect_timeout} seconds "
                         f"({i} of {creds.connect_retries})"
                     )
@@ -586,14 +576,27 @@
         else:
             raise exc
 
         connection.handle = handle
         connection.state = ConnectionState.OPEN
         return connection
 
+    @classmethod
+    def data_type_code_to_name(cls, type_code: Union[type, str]) -> str:  # type: ignore
+        """
+        :param Union[type, str] type_code: The sql to execute.
+            * type_code is a python type (!) in pyodbc https://github.com/mkleehammer/pyodbc/wiki/Cursor#description, and a string for other spark runtimes.
+            * ignoring the type annotation on the signature for this adapter instead of updating the base class because this feels like a really special case.
+        :return: stringified the cursor type_code
+        :rtype: str
+        """
+        if isinstance(type_code, str):
+            return type_code
+        return type_code.__name__.upper()
+
 
 def build_ssl_transport(host, port, username, auth, kerberos_service_name, password=None):
     transport = None
     if port is None:
         port = 10000
     if auth is None:
         auth = "NONE"
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.5.0/dbt/adapters/spark/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import re
 from concurrent.futures import Future
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Set, Tuple, Union, Callable
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Union, Type, Tuple, Callable
 from typing_extensions import TypeAlias
 from dbt.contracts.graph.manifest import Manifest
 
 import agate
 from agate import Table
 
 from dbt.contracts.relation import RelationType
 
 import dbt
 import dbt.exceptions
 
-from dbt.adapters.base import AdapterConfig
+from dbt.adapters.base import AdapterConfig, PythonJobHelper
 from dbt.adapters.base.impl import catch_as_completed
-from dbt.events.functions import fire_event
-from dbt.events.types import ListRelations
-from dbt.adapters.cache import _make_key
+from dbt.contracts.connection import AdapterResponse
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.spark import SparkConnectionManager
 from dbt.adapters.spark import SparkRelation
 from dbt.adapters.spark import SparkColumn
-from dbt.adapters.spark.spark_utils import is_openhouse
+from dbt.adapters.spark.python_submissions import (
+    JobClusterPythonJobHelper,
+    AllPurposeClusterPythonJobHelper,
+)
 from dbt.adapters.base import BaseRelation, available
 from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt.events import AdapterLogger
+from dbt.flags import get_flags
 from dbt.utils import executor, AttrDict
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
 
 logger = AdapterLogger("Spark")
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
@@ -59,15 +61,14 @@
 class PartitionConfig(dbtClassMixin):
     field: str
     data_type: str
     granularity: Optional[str] = None
 
     @classmethod
     def parse(cls, partition_by) -> Optional["PartitionConfig"]:
-
         if partition_by is None:
             return None
         try:
             cls.validate(partition_by)
             return cls.from_dict(partition_by)
         except ValidationError as exc:
             raise dbt.exceptions.ValidationException("Could not parse partition config") from exc
@@ -157,94 +158,71 @@
     def quote(self, identifier):
         return "`{}`".format(identifier)
 
     def add_schema_to_cache(self, schema) -> str:
         """Cache a new schema in dbt. It will show up in `list relations`."""
         if schema is None:
             name = self.nice_connection_name()
-            dbt.exceptions.raise_compiler_error(
+            raise dbt.exceptions.CompilationError(
                 "Attempted to cache a null schema for {}".format(name)
             )
-        if dbt.flags.USE_CACHE:
+        if get_flags().USE_CACHE:  # type: ignore
             self.cache.add_schema(None, schema)
         # so jinja doesn't render things
         return ""
 
     def _get_relation_information(
         self, schema_relation: BaseRelation, row: agate.Row
     ) -> RelationInfo:
         """relation info was fetched with SHOW TABLES EXTENDED"""
         try:
             _schema, name, _, information = row
         except ValueError:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f'Invalid value from "show tables extended ...", got {len(row)} values, expected 4'
             )
 
         return schema_relation.database, _schema, name, information
 
     def _get_relation_information_using_describe(
         self, schema_relation: BaseRelation, row: agate.Row
     ) -> RelationInfo:
         """Relation info fetched using SHOW TABLES and an auxiliary DESCRIBE statement"""
         try:
             _schema, name = row
         except ValueError:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f'Invalid value from "show tables ...", got {len(row)} values, expected 2'
             )
 
+        is_openhouse = schema_relation.database == "openhouse" or "." in schema_relation.schema
+
         # database is needed where relations can exist in different catalogs
         table_name = f"{_schema}.{name}"
-        if is_openhouse(schema_relation.database, schema_relation.schema):
+        if is_openhouse:
             if not table_name.startswith("openhouse."):
                 table_name = "openhouse." + table_name
             _schema = "openhouse." + _schema
 
         try:
             table_results = self.execute_macro(
                 DESCRIBE_TABLE_EXTENDED_MACRO_NAME, kwargs={"table_name": table_name}
             )
-        except dbt.exceptions.RuntimeException as e:
+        except dbt.exceptions.DbtRuntimeError as e:
             logger.debug(f"Error while retrieving information about {table_name}: {e.msg}")
             table_results = AttrDict()
 
         information = ""
         for info_row in table_results:
             info_type, info_value, _ = info_row
             if not info_type.startswith("#"):
                 information += f"{info_type}: {info_value}\n"
 
         return schema_relation.database, _schema, name, information
 
-    def _get_relation_map(self, manifest: Manifest) -> Dict[str, List[BaseRelation]]:
-        """Relations compiled together based on schema"""
-        relations = [
-            self.Relation.create_from(self.config, node)  # keep the identifier
-            for node in manifest.nodes.values()
-            if (node.is_relational and not node.is_ephemeral_model)
-        ]
-        sources = [
-            self.Relation.create_from(self.config, node)  # keep the identifier
-            for node in manifest.sources.values()
-        ]
-
-        import collections
-
-        relation_map = collections.defaultdict(list)
-        for r in relations:
-            relation_map[r.schema].append(r)
-        for s in sources:
-            if s.database == "openhouse" and "." not in s.schema:
-                relation_map[s.database + "." + s.schema].append(s)
-            else:
-                relation_map[s.schema].append(s)
-
-        return relation_map
-
     def _build_spark_relation_list(
         self,
         schema_relation: BaseRelation,
         row_list: agate.Table,
         relation_info_func: Callable[[BaseRelation, agate.Row], RelationInfo],
     ) -> List[BaseRelation]:
         """Aggregate relations with format metadata included."""
@@ -257,15 +235,15 @@
             )
             is_delta: bool = "Provider: delta" in information
             is_hudi: bool = "Provider: hudi" in information
             is_iceberg: bool = "Provider: iceberg" in information
             is_openhouse: bool = "Provider: openhouse" in information
 
             relation: BaseRelation = self.Relation.create(  # type: ignore
-                database=database if database and not _schema.startswith("openhouse.") else None,
+                database=database if database else None,
                 schema=_schema,
                 identifier=name,
                 type=rel_type,
                 information=information,
                 is_delta=is_delta,
                 is_iceberg=is_iceberg,
                 is_hudi=is_hudi,
@@ -277,16 +255,18 @@
 
     def list_relations_without_caching(self, schema_relation: BaseRelation) -> List[BaseRelation]:
         """Distinct Spark compute engines may not support the same SQL featureset. Thus, we must
         try different methods to fetch relation information."""
 
         kwargs = {"schema_relation": schema_relation}
 
+        is_openhouse = schema_relation.database == "openhouse" or "." in schema_relation.schema
+
         try:
-            if is_openhouse(schema_relation.database, schema_relation.schema):
+            if is_openhouse:
                 # Iceberg behavior: 3-row result of relations obtained
                 show_table_rows = self.execute_macro(
                     LIST_RELATIONS_SHOW_TABLES_MACRO_NAME, kwargs=kwargs
                 )
                 return self._build_spark_relation_list(
                     schema_relation=schema_relation,
                     row_list=show_table_rows,
@@ -298,15 +278,15 @@
                         LIST_RELATIONS_MACRO_NAME, kwargs=kwargs
                     )
                     return self._build_spark_relation_list(
                         schema_relation=schema_relation,
                         row_list=show_table_extended_rows,
                         relation_info_func=self._get_relation_information,
                     )
-        except dbt.exceptions.RuntimeException as e:
+        except dbt.exceptions.DbtRuntimeError as e:
             errmsg = getattr(e, "msg", "")
             print(errmsg)
             if f"Database '{schema_relation}' not found" in errmsg:
                 return []
             # Iceberg compute engine behavior: show table
             elif "SHOW TABLE EXTENDED is not supported for v2 tables" in errmsg:
                 # this happens with spark-iceberg with v2 iceberg tables
@@ -317,36 +297,34 @@
                         LIST_RELATIONS_SHOW_TABLES_MACRO_NAME, kwargs=kwargs
                     )
                     return self._build_spark_relation_list(
                         schema_relation=schema_relation,
                         row_list=show_table_rows,
                         relation_info_func=self._get_relation_information_using_describe,
                     )
-                except dbt.exceptions.RuntimeException as e:
+                except dbt.exceptions.DbtRuntimeError as e:
                     description = "Error while retrieving information about"
                     logger.debug(f"{description} {schema_relation}: {e.msg}")
                     return []
             else:
                 logger.debug(
                     f"Error while retrieving information about {schema_relation}: {errmsg}"
                 )
                 return []
 
-    def get_relation(
-        self, database: Optional[str], schema: str, identifier: str
-    ) -> Optional[BaseRelation]:
-        if not self.Relation.include_policy.database:
-            database = None
+    def get_relation(self, database: str, schema: str, identifier: str) -> Optional[BaseRelation]:
+        if not self.Relation.get_default_include_policy().database:
+            database = None  # type: ignore
         else:
             database = database if database else None
 
         return super().get_relation(database, schema, identifier)
 
     def parse_describe_extended(
-        self, relation: Relation, raw_rows: List[agate.Row]
+        self, relation: BaseRelation, raw_rows: AttrDict
     ) -> List[SparkColumn]:
         # Convert the Row to a dict
         dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
         # Find the separator between the rows and the metadata provided
         # by the DESCRIBE TABLE EXTENDED statement
         pos = self.find_table_information_separator(dict_rows)
 
@@ -377,57 +355,45 @@
         pos = 0
         for row in rows:
             if not row["col_name"] or row["col_name"].startswith("#"):
                 break
             pos += 1
         return pos
 
-    def get_columns_in_relation(self, relation: Relation) -> List[SparkColumn]:
-        cached_relations = self.cache.get_relations(relation.database, relation.schema)
-        cached_relation = next(
-            (
-                cached_relation
-                for cached_relation in cached_relations
-                if str(cached_relation) == str(relation)
-            ),
-            None,
-        )
+    def get_columns_in_relation(self, relation: BaseRelation) -> List[SparkColumn]:
         columns = []
-        if cached_relation and cached_relation.information:
-            columns = self.parse_columns_from_information(cached_relation)
-        if not columns:
-            # in open source delta 'show table extended' query output doesnt
-            # return relation's schema. if columns are empty from cache,
-            # use get_columns_in_relation spark macro
-            # which would execute 'describe extended tablename' query
-            try:
-                rows: List[agate.Row] = self.execute_macro(
-                    GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME, kwargs={"relation": relation}
-                )
-                columns = self.parse_describe_extended(relation, rows)
-            except dbt.exceptions.RuntimeException as e:
-                # spark would throw error when table doesn't exist, where other
-                # CDW would just return and empty list, normalizing the behavior here
-                errmsg = getattr(e, "msg", "")
-                found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
-                if any(found_msgs):
-                    pass
-                else:
-                    raise e
+        try:
+            rows: AttrDict = self.execute_macro(
+                GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME, kwargs={"relation": relation}
+            )
+            columns = self.parse_describe_extended(relation, rows)
+        except dbt.exceptions.DbtRuntimeError as e:
+            # spark would throw error when table doesn't exist, where other
+            # CDW would just return and empty list, normalizing the behavior here
+            errmsg = getattr(e, "msg", "")
+            found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
+            if any(found_msgs):
+                pass
+            else:
+                raise e
 
         # strip hudi metadata columns.
         columns = [x for x in columns if x.name not in self.HUDI_METADATA_COLUMNS]
         return columns
 
-    def parse_columns_from_information(self, relation: SparkRelation) -> List[SparkColumn]:
-        owner_match = re.findall(self.INFORMATION_OWNER_REGEX, relation.information)
+    def parse_columns_from_information(self, relation: BaseRelation) -> List[SparkColumn]:
+        if hasattr(relation, "information"):
+            information = relation.information or ""
+        else:
+            information = ""
+        owner_match = re.findall(self.INFORMATION_OWNER_REGEX, information)
         owner = owner_match[0] if owner_match else None
-        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, relation.information)
+        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, information)
         columns = []
-        stats_match = re.findall(self.INFORMATION_STATISTICS_REGEX, relation.information)
+        stats_match = re.findall(self.INFORMATION_STATISTICS_REGEX, information)
         raw_table_stats = stats_match[0] if stats_match else None
         table_stats = SparkColumn.convert_table_stats(raw_table_stats)
         for match_num, match in enumerate(matches):
             column_name, column_type, nullable = match.groups()
             column = SparkColumn(
                 table_database=relation.database,
                 table_schema=relation.schema,
@@ -438,33 +404,15 @@
                 column=column_name,
                 dtype=column_type,
                 table_stats=table_stats,
             )
             columns.append(column)
         return columns
 
-    # overriding this method to optimize the performance of list_relations_without_caching
-    def _get_cache_schemas(self, manifest: Manifest) -> Set[BaseRelation]:
-        """Get the set of schema relations that the cache logic needs to
-        populate. This means only executable nodes are included.
-        """
-        relation_map = self._get_relation_map(manifest)
-
-        schemas = [
-            self.Relation.create(
-                schema=schema,
-                identifier=(
-                    "|".join(r.identifier for r in relations) if len(relations) < 100 else "*"
-                ),
-            )
-            for schema, relations in relation_map.items()
-        ]
-        return set(schemas)
-
-    def _get_columns_for_catalog(self, relation: SparkRelation) -> Iterable[Dict[str, Any]]:
+    def _get_columns_for_catalog(self, relation: BaseRelation) -> Iterable[Dict[str, Any]]:
         columns = self.parse_columns_from_information(relation)
 
         if not columns:
             # Columns are empty for openhouse, since it's trying to parse using spark logic
             logger.info(
                 "parse_columns_from_information doesn't return any columns, format may be openhouse"
                 "Trying to fetch and parse using openhouse format"
@@ -492,39 +440,42 @@
 
         with executor(self.config) as tpe:
             futures: List[Future[Table]] = []
             for info, schemas in schema_map.items():
                 for schema in schemas:
                     futures.append(
                         tpe.submit_connected(
-                            self, schema, self._get_one_catalog, info, [schema], manifest
+                            self,
+                            schema,
+                            self._get_one_catalog,
+                            info,
+                            [schema],
+                            manifest,
                         )
                     )
             catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
     def _get_one_catalog(
         self,
         information_schema,
         schemas,
         manifest,
     ) -> agate.Table:
         if len(schemas) != 1:
-            dbt.exceptions.raise_compiler_error(
+            raise dbt.exceptions.CompilationError(
                 f"Expected only one schema in spark _get_one_catalog, found " f"{schemas}"
             )
 
         database = information_schema.database
         schema = list(schemas)[0]
 
-        relation_map = self._get_relation_map(manifest)
-
         columns: List[Dict[str, Any]] = []
-        for relation in self.list_relations(database, schema, relation_map=relation_map):
-            logger.debug("Getting table schema for relation {}", relation)
+        for relation in self.list_relations(database, schema):
+            logger.debug("Getting table schema for relation {}", str(relation))
             columns.extend(self._get_columns_for_catalog(relation))
         return agate.Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
 
     def list_schemas(self, database: str) -> List[str]:
         connection = self.connections.get_if_exists()
         if connection is not None:
             database = connection.credentials.database
@@ -539,44 +490,14 @@
 
         # The catalog for `show table extended` needs to match the current catalog.
         with self._catalog(database):
             results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": schema})
         schema_list = [row[0] for row in results]
         return schema_list
 
-    def list_relations(self, database: Optional[str], schema: str, **kwargs) -> List[BaseRelation]:
-        if self._schema_is_cached(database, schema):
-            return self.cache.get_relations(database, schema)
-
-        relation_map = kwargs.get("relation_map", None)
-
-        if relation_map:
-            if database == "openhouse" and "." not in schema:
-                schema = f"{database}.{schema}"
-
-        schema_relation = self.Relation.create(
-            database=database,
-            schema=schema,
-            identifier="|".join(r.identifier for r in relation_map[schema])
-            if relation_map
-            else "",
-            quote_policy=self.config.quoting,
-        )
-
-        # we can't build the relations cache because we don't have a
-        # manifest so we can't run any operations.
-        relations = self.list_relations_without_caching(schema_relation)
-        fire_event(
-            ListRelations(
-                database=database, schema=schema, relations=[_make_key(x) for x in relations]
-            )
-        )
-
-        return relations
-
     def check_schema_exists(self, database, schema):
         # in case the user is using "openhouse" as a catalog, the format of schema will be 'openhouse.db'.
         # so derive the catalog/database value from schema until we support `openhouse` catalog natively.
         if schema is not None and "." in schema:
             tokens = schema.split(".")
             database = tokens[0]
             schema = tokens[1]
@@ -634,14 +555,28 @@
         except BaseException as e:
             print(sql)
             print(e)
             raise
         finally:
             conn.transaction_open = False
 
+    def generate_python_submission_response(self, submission_result: Any) -> AdapterResponse:
+        return self.connections.get_response(None)
+
+    @property
+    def default_python_submission_method(self) -> str:
+        return "all_purpose_cluster"
+
+    @property
+    def python_submission_helpers(self) -> Dict[str, Type[PythonJobHelper]]:
+        return {
+            "job_cluster": JobClusterPythonJobHelper,
+            "all_purpose_cluster": AllPurposeClusterPythonJobHelper,
+        }
+
     def standardize_grants_dict(self, grants_table: agate.Table) -> dict:
         grants_dict: Dict[str, List[str]] = {}
         for row in grants_table:
             grantee = row["Principal"]
             privilege = row["ActionType"]
             object_type = row["ObjectType"]
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.5.0/dbt/adapters/spark/relation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Optional, Dict, Any
-
-from dataclasses import dataclass
+from typing import Optional, TypeVar, Dict, Any
+from dataclasses import dataclass, field
 
 from dbt.adapters.base.relation import BaseRelation, Policy
 
 from dbt.adapters.spark.spark_utils import remove_undefined
 
+from dbt.events import AdapterLogger
+
+logger = AdapterLogger("Spark")
+
+Self = TypeVar("Self", bound="BaseRelation")
+
 
 @dataclass
 class SparkQuotePolicy(Policy):
     database: bool = False
     schema: bool = False
     identifier: bool = False
 
@@ -19,16 +24,16 @@
     database: bool = True
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class SparkRelation(BaseRelation):
-    quote_policy: SparkQuotePolicy = SparkQuotePolicy()
-    include_policy: SparkIncludePolicy = SparkIncludePolicy()
+    quote_policy: Policy = field(default_factory=lambda: SparkQuotePolicy())
+    include_policy: Policy = field(default_factory=lambda: SparkIncludePolicy())
     quote_character: str = "`"
     is_delta: Optional[bool] = None
     is_hudi: Optional[bool] = None
     is_iceberg: Optional[bool] = None
     # TODO: make this a dict everywhere
     is_openhouse: Optional[bool] = None
     information: Optional[str] = None
```

### Comparing `in-dbt-spark-1.2.521/dbt/adapters/spark/session.py` & `in-dbt-spark-1.5.0/dbt/adapters/spark/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             The first row.
 
         Source
         ------
         https://github.com/mkleehammer/pyodbc/wiki/Cursor#fetchone
         """
         if self._rows is None and self._df is not None:
-            self._rows = self._df.collect()
+            self._rows = self._df.take(1)
 
         if self._rows is not None and len(self._rows) > 0:
             row = self._rows.pop(0)
         else:
             row = None
 
         return row
```

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/adapters.sql`

 * *Files 9% similar despite different names*

```diff
@@ -74,37 +74,14 @@
       comment '{{ model.description | replace("'", "\\'") }}'
     {% endif %}
   {%- elif raw_persist_docs -%}
     {{ exceptions.raise_compiler_error("Invalid value provided for 'persist_docs'. Expected dict but got value: " ~ raw_persist_docs) }}
   {% endif %}
 {%- endmacro -%}
 
-{% macro set_dbt_tblproperties(relation, model) %}
-  {{ return(adapter.dispatch('set_dbt_tblproperties', 'dbt')(relation, model)) }}
-{%- endmacro -%}
-
-{% macro spark__set_dbt_tblproperties(relation, model) %}
-  {%- set mp_name = var('MULTIPRODUCT_NAME', None) -%}
-  {%- set project_name = model.package_name -%}
-  {%- set model_name = model.name -%}
-
-  {% if target.name == 'prod' and config.get('file_format', 'openhouse') == 'openhouse' %}
-    {% set set_tblproperties_query %}
-        {% if mp_name is not none %}
-            alter table {{ relation }} set tblproperties ('dbt.mp_name'='{{ mp_name }}',
-                                                          'dbt.project_name'='{{ project_name }}',
-                                                          'dbt.model_name'='{{ model_name }}');
-        {% else %}
-            alter table {{ relation }} set tblproperties ('dbt.project_name'='{{ project_name }}',
-                                                          'dbt.model_name'='{{ model_name }}');
-        {% endif %}
-    {% endset %}
-    {% do run_query(set_tblproperties_query) %}
-  {% endif %}
-{% endmacro %}
 
 {% macro partition_cols(label, required=false) %}
   {{ return(adapter.dispatch('partition_cols', 'dbt')(label, required)) }}
 {%- endmacro -%}
 
 {% macro spark__partition_cols(label, required=false) %}
   {%- set raw_partition_by = config.get('partition_by', validator=validation.any[list, dict]) -%}
@@ -115,15 +92,15 @@
     {%- set partition_by_list = adapter.parse_partition_by(raw_partition_by) -%}
     {%- for partition_by in partition_by_list -%}
       {%- if file_format == 'openhouse' and partition_by.data_type | lower in ['timestamp'] -%}
         {%- if partition_by.granularity is none -%}
           {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse' and data_type = 'timestamp', granularity must be provided") %}
         {%- endif -%}
         {{ partition_by.granularity }}({{ partition_by.field }})
-      {%- elif file_format == 'openhouse' and partition_by.data_type | lower in ['string', 'int'] -%}
+      {%- elif file_format == 'openhouse' and partition_by.data_type | lower in ['string'] -%}
         {{ partition_by.field }}
       {%- else -%}
         {{ partition_by.field }}
       {%- endif -%}
       {%- if not loop.last -%},{%- endif -%}
     {%- endfor -%}
     )
@@ -155,53 +132,124 @@
   {% call statement('list_properties', fetch_result=True) -%}
     SHOW TBLPROPERTIES {{ relation }}
   {% endcall %}
   {% do return(load_result('list_properties').table) %}
 {%- endmacro %}
 
 
-{% macro create_temporary_view(relation, sql) -%}
-  {{ return(adapter.dispatch('create_temporary_view', 'dbt')(relation, sql)) }}
+{% macro create_temporary_view(relation, compiled_code) -%}
+  {{ return(adapter.dispatch('create_temporary_view', 'dbt')(relation, compiled_code)) }}
 {%- endmacro -%}
 
-{#-- We can't use temporary tables with `create ... as ()` syntax #}
-{% macro spark__create_temporary_view(relation, sql) -%}
-  create temporary view {{ relation.include(schema=false) }} as
-    {{ sql }}
+{#-- We can't use temporary tables with `create ... as ()` syntax --#}
+{% macro spark__create_temporary_view(relation, compiled_code) -%}
+    create temporary view {{ relation }} as
+      {{ compiled_code }}
+{%- endmacro -%}
+
+
+{%- macro spark__create_table_as(temporary, relation, compiled_code, language='sql') -%}
+  {%- if language == 'sql' -%}
+    {%- if temporary -%}
+      {{ create_temporary_view(relation, compiled_code) }}
+    {%- else -%}
+      {% if config.get('file_format', validator=validation.any[basestring]) in ['delta', 'iceberg'] %}
+        create or replace table {{ relation }}
+      {% else %}
+        create table {{ relation }}
+      {% endif %}
+      {%- set contract_config = config.get('contract') -%}
+      {%- if contract_config.enforced -%}
+        {{ get_assert_columns_equivalent(compiled_code) }}
+        {%- set compiled_code = get_select_subquery(compiled_code) %}
+      {% endif %}
+      {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
+        {{ file_format_clause() }}
+      {% endif %}
+      {{ options_clause() }}
+      {{ partition_cols(label="partitioned by") }}
+      {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
+        {{ clustered_cols(label="clustered by") }}
+        {{ location_clause() }}
+      {% endif %}
+      {{ comment_clause() }}
+      as
+      {{ compiled_code }}
+    {%- endif -%}
+  {%- elif language == 'python' -%}
+    {#--
+    N.B. Python models _can_ write to temp views HOWEVER they use a different session
+    and have already expired by the time they need to be used (I.E. in merges for incremental models)
+
+    TODO: Deep dive into spark sessions to see if we can reuse a single session for an entire
+    dbt invocation.
+     --#}
+    {{ py_write_table(compiled_code=compiled_code, target_relation=relation) }}
+  {%- endif -%}
+{%- endmacro -%}
+
+
+{% macro persist_constraints(relation, model) %}
+  {{ return(adapter.dispatch('persist_constraints', 'dbt')(relation, model)) }}
 {% endmacro %}
 
+{% macro spark__persist_constraints(relation, model) %}
+  {%- set contract_config = config.get('contract') -%}
+  {% if contract_config.enforced and config.get('file_format', 'delta') == 'delta' %}
+    {% do alter_table_add_constraints(relation, model.columns) %}
+    {% do alter_column_set_constraints(relation, model.columns) %}
+  {% endif %}
+{% endmacro %}
 
-{% macro spark__create_table_as(temporary, relation, sql) -%}
-  {% if temporary -%}
-    {{ create_temporary_view(relation, sql) }}
-  {%- else -%}
-    {% if config.get('file_format', validator=validation.any[basestring]) in ['delta', 'iceberg'] %}
-      create or replace table {{ relation }}
-    {% else %}
-      create table {{ relation }}
-    {% endif %}
-    {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
-      {{ file_format_clause() }}
-    {% endif %}
-    {{ options_clause() }}
-    {{ partition_cols(label="partitioned by") }}
-    {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
-      {{ clustered_cols(label="clustered by") }}
-      {{ location_clause() }}
-    {% endif %}
-    {{ comment_clause() }}
-    as
-      {{ sql }}
+{% macro alter_table_add_constraints(relation, constraints) %}
+  {{ return(adapter.dispatch('alter_table_add_constraints', 'dbt')(relation, constraints)) }}
+{% endmacro %}
 
-  {%- endif %}
-{%- endmacro -%}
+{% macro spark__alter_table_add_constraints(relation, column_dict) %}
+
+  {% for column_name in column_dict %}
+    {% set constraints = column_dict[column_name]['constraints'] %}
+    {% for constraint in constraints %}
+      {% if constraint.type == 'check' and not is_incremental() %}
+        {%- set constraint_hash = local_md5(column_name ~ ";" ~ constraint.expression ~ ";" ~ loop.index) -%}
+        {% call statement() %}
+          alter table {{ relation }} add constraint {{ constraint_hash }} check {{ constraint.expression }};
+        {% endcall %}
+      {% endif %}
+    {% endfor %}
+  {% endfor %}
+{% endmacro %}
+
+{% macro alter_column_set_constraints(relation, column_dict) %}
+  {{ return(adapter.dispatch('alter_column_set_constraints', 'dbt')(relation, column_dict)) }}
+{% endmacro %}
+
+{% macro spark__alter_column_set_constraints(relation, column_dict) %}
+  {% for column_name in column_dict %}
+    {% set constraints = column_dict[column_name]['constraints'] %}
+    {% for constraint in constraints %}
+      {% if constraint.type != 'not_null' %}
+        {{ exceptions.warn('Invalid constraint for column ' ~ column_name ~ '. Only `not_null` is supported.') }}
+      {% else %}
+        {% set quoted_name = adapter.quote(column_name) if column_dict[column_name]['quote'] else column_name %}
+        {% call statement() %}
+          alter table {{ relation }} change column {{ quoted_name }} set not null {{ constraint.expression or "" }};
+        {% endcall %}
+      {% endif %}
+    {% endfor %}
+  {% endfor %}
+{% endmacro %}
 
 {% macro spark__create_view_as(relation, sql) -%}
   create or replace view {{ relation }}
   {{ comment_clause() }}
+  {%- set contract_config = config.get('contract') -%}
+  {%- if contract_config.enforced -%}
+    {{ get_assert_columns_equivalent(sql) }}
+  {%- endif %}
   as
     {{ sql }}
 {% endmacro %}
 
 {% macro spark__create_schema(relation) -%}
   {%- call statement('create_schema') -%}
     {% if '.' in relation.schema %}
@@ -224,15 +272,15 @@
 
 {% macro get_columns_in_relation_raw(relation) -%}
   {{ return(adapter.dispatch('get_columns_in_relation_raw', 'dbt')(relation)) }}
 {%- endmacro -%}
 
 {% macro spark__get_columns_in_relation_raw(relation) -%}
   {% call statement('get_columns_in_relation_raw', fetch_result=True) %}
-      describe extended {{ relation.include(schema=(schema is not none)) }}
+      describe extended {{ relation }}
   {% endcall %}
   {% do return(load_result('get_columns_in_relation_raw').table) %}
 {% endmacro %}
 
 {% macro spark__get_columns_in_relation(relation) -%}
   {% call statement('get_columns_in_relation', fetch_result=True) %}
       describe extended {{ relation.include(schema=(schema is not none)) }}
@@ -249,15 +297,15 @@
 {% endmacro %}
 
 {% macro list_relations_show_tables_without_caching(schema_relation) %}
   {#-- Spark with iceberg tables don't work with show table extended for #}
   {#-- V2 iceberg tables #}
   {#-- https://issues.apache.org/jira/browse/SPARK-33393 #}
   {% call statement('list_relations_without_caching_show_tables', fetch_result=True) -%}
-    show tables in {{ schema_relation.schema }} like '{{ schema_relation.identifier or "*" }}'
+    show tables in {{ schema_relation }} like '*'
   {% endcall %}
 
   {% do return(load_result('list_relations_without_caching_show_tables').table) %}
 {% endmacro %}
 
 {% macro describe_table_extended_without_caching(table_name) %}
   {#-- Spark with iceberg tables don't work with show table extended for #}
@@ -273,18 +321,14 @@
 {% macro spark__list_schemas(database) -%}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) %}
     show databases like '{{ database or "*" }}'
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
 
-{% macro spark__current_timestamp() -%}
-  current_timestamp()
-{%- endmacro %}
-
 {% macro spark__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
     {% if not from_relation.type %}
       {% do exceptions.raise_database_error("Cannot rename a relation with a blank type: " ~ from_relation.identifier) %}
     {% elif from_relation.type in ('table') %}
         alter table {{ from_relation }} rename to {{ to_relation }}
     {% elif from_relation.type == 'view' %}
@@ -358,16 +402,15 @@
     {% do run_query(comment_query) %}
   {% endif %}
 {% endmacro %}
 
 {% macro spark__make_temp_relation(base_relation, suffix) %}
     {% set tmp_identifier = base_relation.identifier ~ suffix %}
     {% set tmp_relation = base_relation.incorporate(path = {
-        "identifier": tmp_identifier,
-        "schema": None
+        "identifier": tmp_identifier
     }) -%}
 
     {% do return(tmp_relation) %}
 {% endmacro %}
 
 
 {% macro spark__alter_column_type(relation, column_name, new_column_type) -%}
@@ -406,89 +449,7 @@
             {% endfor %}
 
   {%- endset -%}
 
   {% do run_query(sql) %}
 
 {% endmacro %}
-
-
-{% macro spark__get_binding_char() %}
-  {{ return('?' if target.method == 'odbc' else '%s') }}
-{% endmacro %}
-
-
-{% macro spark__reset_csv_table(model, full_refresh, old_relation, agate_table) %}
-    {% if old_relation %}
-        {{ adapter.drop_relation(old_relation) }}
-    {% endif %}
-    {% set sql = create_csv_table(model, agate_table) %}
-    {{ return(sql) }}
-{% endmacro %}
-
-
-{% macro spark__load_csv_rows(model, agate_table) %}
-
-  {% set batch_size = get_batch_size() %}
-  {% set column_override = model['config'].get('column_types', {}) %}
-
-  {% set statements = [] %}
-
-  {% for chunk in agate_table.rows | batch(batch_size) %}
-      {% set bindings = [] %}
-
-      {% for row in chunk %}
-          {% do bindings.extend(row) %}
-      {% endfor %}
-
-      {% set sql %}
-          insert into {{ this.render() }} values
-          {% for row in chunk -%}
-              ({%- for col_name in agate_table.column_names -%}
-                  {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
-                  {%- set type = column_override.get(col_name, inferred_type) -%}
-                    {# todo- https://jira01.corp.linkedin.com:8443/browse/DATAFND-660 #}
-                    cast('{{ row.get(col_name) if row.get(col_name) is not none else null }}' as {{type}})
-                  {%- if not loop.last%},{%- endif %}
-              {%- endfor -%})
-              {%- if not loop.last%},{%- endif %}
-          {%- endfor %}
-      {% endset %}
-
-      {% do adapter.add_query(sql, bindings=bindings, abridge_sql_log=True) %}
-
-      {% if loop.index0 == 0 %}
-          {% do statements.append(sql) %}
-      {% endif %}
-  {% endfor %}
-
-  {# Return SQL so we can render it out into the compiled files #}
-  {{ return(statements[0]) }}
-{% endmacro %}
-
-
-{% macro spark__create_csv_table(model, agate_table) %}
-  {%- set column_override = model['config'].get('column_types', {}) -%}
-  {%- set quote_seed_column = model['config'].get('quote_columns', None) -%}
-
-  {% set sql %}
-    create table {{ this.render() }} (
-        {%- for col_name in agate_table.column_names -%}
-            {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
-            {%- set type = column_override.get(col_name, inferred_type) -%}
-            {%- set column_name = (col_name | string) -%}
-            {{ adapter.quote_seed_column(column_name, quote_seed_column) }} {{ type }} {%- if not loop.last -%}, {%- endif -%}
-        {%- endfor -%}
-    )
-    {{ file_format_clause() }}
-    {{ partition_cols(label="partitioned by") }}
-    {{ clustered_cols(label="clustered by") }}
-    {{ location_clause() }}
-    {{ comment_clause() }}
-  {% endset %}
-
-  {% call statement('_') -%}
-    {{ sql }}
-  {%- endcall %}
-
-  {{ return(sql) }}
-{% endmacro %}
```

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/apply_retention.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/apply_retention.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files 7% similar despite different names*

```diff
@@ -6,33 +6,36 @@
       {# removed table from statement for iceberg #}
       insert overwrite {{ target_relation }}
       {# removed partition_cols for iceberg as well #}
     {% else %}
       insert overwrite table {{ target_relation }}
       {{ partition_cols(label="partition") }}
     {% endif %}
-    select {{dest_cols_csv}} from {{ source_relation.include(database=false, schema=false) }}
+    select {{dest_cols_csv}} from {{ source_relation }}
 
 {% endmacro %}
 
 
 {% macro get_insert_into_sql(source_relation, target_relation) %}
 
     {%- set dest_columns = adapter.get_columns_in_relation(target_relation) -%}
     {%- set dest_cols_csv = dest_columns | map(attribute='quoted') | join(', ') -%}
     insert into table {{ target_relation }}
-    select {{dest_cols_csv}} from {{ source_relation.include(database=false, schema=false) }}
+    select {{dest_cols_csv}} from {{ source_relation }}
 
 {% endmacro %}
 
 
-{% macro spark__get_merge_sql(target, source, unique_key, dest_columns, predicates=none) %}
-  {# skip dest_columns, use merge_update_columns config if provided, otherwise use "*" #}
-  {%- set predicates = [] if predicates is none else [] + predicates -%}
-  {%- set update_columns = config.get("merge_update_columns") -%}
+{% macro spark__get_merge_sql(target, source, unique_key, dest_columns, incremental_predicates) %}
+  {# need dest_columns for merge_exclude_columns, default to use "*" #}
+  {%- set predicates = [] if incremental_predicates is none else [] + incremental_predicates -%}
+  {%- set dest_columns = adapter.get_columns_in_relation(target) -%}
+  {%- set merge_update_columns = config.get('merge_update_columns') -%}
+  {%- set merge_exclude_columns = config.get('merge_exclude_columns') -%}
+  {%- set update_columns = get_merge_update_columns(merge_update_columns, merge_exclude_columns, dest_columns) -%}
 
   {% if unique_key %}
       {% if unique_key is sequence and unique_key is not mapping and unique_key is not string %}
           {% for key in unique_key %}
               {% set this_key_match %}
                   DBT_INTERNAL_SOURCE.{{ key }} = DBT_INTERNAL_DEST.{{ key }}
               {% endset %}
@@ -47,38 +50,38 @@
   {% else %}
       {% do predicates.append('FALSE') %}
   {% endif %}
 
   {{ sql_header if sql_header is not none }}
 
   merge into {{ target }} as DBT_INTERNAL_DEST
-      using {{ source.include(schema=false) }} as DBT_INTERNAL_SOURCE
+      using {{ source }} as DBT_INTERNAL_SOURCE
       on {{ predicates | join(' and ') }}
 
       when matched then update set
         {% if update_columns -%}{%- for column_name in update_columns %}
             {{ column_name }} = DBT_INTERNAL_SOURCE.{{ column_name }}
             {%- if not loop.last %}, {%- endif %}
         {%- endfor %}
         {%- else %} * {% endif %}
 
       when not matched then insert *
 {% endmacro %}
 
 
-{% macro dbt_spark_get_incremental_sql(strategy, source, target, existing, unique_key) %}
+{% macro dbt_spark_get_incremental_sql(strategy, source, target, existing, unique_key, incremental_predicates) %}
   {%- if strategy == 'append' -%}
     {#-- insert new records into existing table, without updating or overwriting #}
     {{ get_insert_into_sql(source, target) }}
   {%- elif strategy == 'insert_overwrite' -%}
     {#-- insert statements don't like CTEs, so support them via a temp view #}
     {{ get_insert_overwrite_sql(source, target, existing) }}
   {%- elif strategy == 'merge' -%}
   {#-- merge all columns for datasources which implement MERGE INTO (e.g. databricks, iceberg, openhouse) - schema changes are handled for us #}
-    {{ get_merge_sql(target, source, unique_key, dest_columns=none, predicates=none) }}
+    {{ get_merge_sql(target, source, unique_key, dest_columns=none, incremental_predicates=incremental_predicates) }}
   {%- else -%}
     {% set no_sql_for_strategy_msg -%}
       No known SQL for the incremental strategy provided: {{ strategy }}
     {%- endset %}
     {%- do exceptions.raise_compiler_error(no_sql_for_strategy_msg) -%}
   {%- endif -%}
```

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/seed.sql`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,80 @@
-{% materialization seed, adapter = 'spark' %}
+{% macro spark__get_binding_char() %}
+  {{ return('?' if target.method == 'odbc' else '%s') }}
+{% endmacro %}
+
+
+{% macro spark__reset_csv_table(model, full_refresh, old_relation, agate_table) %}
+    {% if old_relation %}
+        {{ adapter.drop_relation(old_relation) }}
+    {% endif %}
+    {% set sql = create_csv_table(model, agate_table) %}
+    {{ return(sql) }}
+{% endmacro %}
+
+
+{% macro spark__load_csv_rows(model, agate_table) %}
+
+  {% set batch_size = get_batch_size() %}
+  {% set column_override = model['config'].get('column_types', {}) %}
+
+  {% set statements = [] %}
+
+  {% for chunk in agate_table.rows | batch(batch_size) %}
+      {% set bindings = [] %}
+
+      {% for row in chunk %}
+          {% do bindings.extend(row) %}
+      {% endfor %}
+
+      {% set sql %}
+          insert into {{ this.render() }} values
+          {% for row in chunk -%}
+              ({%- for col_name in agate_table.column_names -%}
+                  {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
+                  {%- set type = column_override.get(col_name, inferred_type) -%}
+                    {# todo- https://jira01.corp.linkedin.com:8443/browse/DATAFND-660 #}
+                    cast('{{ row.get(col_name) if row.get(col_name) is not none else null }}' as {{type}})
+                  {%- if not loop.last%},{%- endif %}
+              {%- endfor -%})
+              {%- if not loop.last%},{%- endif %}
+          {%- endfor %}
+      {% endset %}
+
+      {% do adapter.add_query(sql, bindings=bindings, abridge_sql_log=True) %}
+
+      {% if loop.index0 == 0 %}
+          {% do statements.append(sql) %}
+      {% endif %}
+  {% endfor %}
+
+  {# Return SQL so we can render it out into the compiled files #}
+  {{ return(statements[0]) }}
+{% endmacro %}
+
+
+{% macro spark__create_csv_table(model, agate_table) %}
+  {%- set column_override = model['config'].get('column_types', {}) -%}
+  {%- set quote_seed_column = model['config'].get('quote_columns', None) -%}
+
+  {% set sql %}
+    create table {{ this.render() }} (
+        {%- for col_name in agate_table.column_names -%}
+            {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
+            {%- set type = column_override.get(col_name, inferred_type) -%}
+            {%- set column_name = (col_name | string) -%}
+            {{ adapter.quote_seed_column(column_name, quote_seed_column) }} {{ type }} {%- if not loop.last -%}, {%- endif -%}
+        {%- endfor -%}
+    )
+    {{ file_format_clause() }}
+    {{ partition_cols(label="partitioned by") }}
+    {{ clustered_cols(label="clustered by") }}
+    {{ location_clause() }}
+    {{ comment_clause() }}
+  {% endset %}
+
+  {% call statement('_') -%}
+    {{ sql }}
+  {%- endcall %}
 
-  {%- set identifier = model['alias'] -%}
-  {%- set full_refresh_mode = (should_full_refresh()) -%}
-
-  {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
-
-  {%- set exists_as_table = (old_relation is not none and old_relation.is_table) -%}
-  {%- set exists_as_view = (old_relation is not none and old_relation.is_view) -%}
-
-  {%- set grant_config = config.get('grants') -%}
-  {%- set agate_table = load_agate_table() -%}
-  -- grab current tables grants config for comparision later on
-
-  {%- do store_result('agate_table', response='OK', agate_table=agate_table) -%}
-
-  {{ run_hooks(pre_hooks, inside_transaction=False) }}
-
-  -- `BEGIN` happens here:
-  {{ run_hooks(pre_hooks, inside_transaction=True) }}
-
-  -- build model
-  {% set create_table_sql = "" %}
-  {% if exists_as_view %}
-    {{ exceptions.raise_compiler_error("Cannot seed to '{}', it is a view".format(old_relation)) }}
-  {% elif exists_as_table %}
-    {% set create_table_sql = reset_csv_table(model, full_refresh_mode, old_relation, agate_table) %}
-  {% else %}
-    {% set create_table_sql = create_csv_table(model, agate_table) %}
-  {% endif %}
-
-  {% set code = 'CREATE' if full_refresh_mode else 'INSERT' %}
-  {% set rows_affected = (agate_table.rows | length) %}
-  {% set sql = load_csv_rows(model, agate_table) %}
-
-  {% call noop_statement('main', code ~ ' ' ~ rows_affected, code, rows_affected) %}
-    {{ get_csv_sql(create_table_sql, sql) }};
-{% endcall %}
-
-  {% set target_relation = this.incorporate(type='table') %}
-
-  {% set should_revoke = should_revoke(old_relation, full_refresh_mode) %}
-  {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
-
-  {% do persist_docs(target_relation, model) %}
-  {% do set_dbt_tblproperties(target_relation, model) %}
-
-  {% if full_refresh_mode or not exists_as_table %}
-    {% do create_indexes(target_relation) %}
-  {% endif %}
-
-  {{ run_hooks(post_hooks, inside_transaction=True) }}
-
-  -- `COMMIT` happens here
-  {{ adapter.commit() }}
-
-  {{ run_hooks(post_hooks, inside_transaction=False) }}
-
-  {{ return({'relations': [target_relation]}) }}
-
-{% endmaterialization %}
+  {{ return(sql) }}
+{% endmacro %}
```

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files 4% similar despite different names*

```diff
@@ -137,19 +137,36 @@
   {%- set target_table = model.get('alias', model.get('name')) -%}
 
   {%- set strategy_name = config.get('strategy') -%}
   {%- set unique_key = config.get('unique_key') %}
   {%- set file_format = config.get('file_format', 'openhouse') -%}
 
   {% set target_relation_exists, target_relation = get_or_create_relation(
-          database=none,
+          database=model.database,
           schema=model.schema,
           identifier=target_table,
           type='table') -%}
 
+  {%- if file_format not in ['delta', 'iceberg', 'hudi', 'openhouse'] -%}
+    {% set invalid_format_msg -%}
+      Invalid file format: {{ file_format }}
+      Snapshot functionality requires file_format be set to 'delta' or 'iceberg' or 'hudi' or 'openhouse'
+    {%- endset %}
+    {% do exceptions.raise_compiler_error(invalid_format_msg) %}
+  {% endif %}
+
+  {%- if target_relation_exists -%}
+    {%- if not target_relation.is_delta and not target_relation.is_iceberg and not target_relation.is_hudi and not target_relation.is_openhouse -%}
+      {% set invalid_format_msg -%}
+        The existing table {{ model.schema }}.{{ target_table }} is in another format than 'delta' or 'iceberg' or 'hudi' or 'openhouse'
+      {%- endset %}
+      {% do exceptions.raise_compiler_error(invalid_format_msg) %}
+    {% endif %}
+  {% endif %}
+
   {% if not adapter.check_schema_exists(model.database, model.schema) %}
     {% do exceptions.raise_compiler_error("Self-serve schema creation is not currently supported in OpenHouse. Please reach out in #ask_openhouse to manually provision your database.") %}
   {% endif %}
 
   {%- if not target_relation.is_table -%}
     {% do exceptions.relation_wrong_type(target_relation, 'table') %}
   {%- endif -%}
@@ -162,15 +179,15 @@
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% set strategy_macro = strategy_dispatch(strategy_name) %}
   {% set strategy = strategy_macro(model, "snapshotted_data", "source_data", config, target_relation_exists) %}
 
   {% if not target_relation_exists %}
 
-      {% set build_sql = build_snapshot_table(strategy, model['compiled_sql']) %}
+      {% set build_sql = build_snapshot_table(strategy, model['compiled_code']) %}
       {% set final_sql = create_table_as(False, target_relation, build_sql) %}
 
   {% else %}
 
       {{ adapter.valid_snapshot_target(target_relation) }}
 
       -- create temp delta table (table_name__dbt_tmp) with changetype as update/insert/delete
@@ -235,15 +252,14 @@
       {{ final_sql }}
   {% endcall %}
 
   {% set should_revoke = should_revoke(target_relation_exists, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
-  {% do set_dbt_tblproperties(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {{ adapter.commit() }}
 
   {% if staging_table is defined %}
       {% do post_snapshot(staging_table) %}
```

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/materializations/validate.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% macro dbt_spark_validate_get_file_format(raw_file_format) %}
   {#-- Validate the file format #}
 
-  {% set accepted_formats = ['text', 'csv', 'json', 'jdbc', 'parquet', 'orc', 'hive', 'delta', 'libsvm', 'hudi', 'iceberg', 'openhouse'] %}
+  {% set accepted_formats = ['text', 'csv', 'json', 'jdbc', 'parquet', 'orc', 'hive', 'delta', 'iceberg', 'libsvm', 'hudi', 'openhouse'] %}
 
   {% set invalid_file_format_msg -%}
     Invalid file format provided: {{ raw_file_format }}
     Expected one of: {{ accepted_formats | join(', ') }}
   {%- endset %}
 
   {% if raw_file_format not in accepted_formats %}
@@ -88,16 +88,16 @@
       {% set partition_by_list = adapter.parse_partition_by(raw_partition_by) %}
       {% if partition_by_list|length > 4 %}
         {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', the size of 'partition_by' must not be > 4.") %}
       {% endif %}
       {% if partition_by_list is not none %}
         {% set timestamp_columns = namespace(count=0) %}
         {%- for partition_by in partition_by_list -%}
-           {%- if partition_by.data_type.lower() not in ['timestamp', 'string', 'int'] -%}
-             {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', 'data_type' must be one of ('timestamp', 'string', 'int').") %}
+           {%- if partition_by.data_type.lower() not in ['timestamp', 'string'] -%}
+             {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', 'data_type' must be one of ('timestamp', 'string').") %}
            {%- endif -%}
            {%- if partition_by.data_type.lower() == 'timestamp' -%}
              {% set timestamp_columns.count = timestamp_columns.count + 1 %}
              {%- if timestamp_columns.count > 1 -%}
                {% do exceptions.raise_compiler_error("For timestamp-partitioned tables with file_format = 'openhouse',
                   OpenHouse only supports 1 timestamp-based column partitioning") %}
              {%- endif -%}
```

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.5.0/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.5.0/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.521/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.5.0/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.521
+Version: 1.5.0
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: ODBC
 Provides-Extra: PyHive
 Provides-Extra: session
 Provides-Extra: all
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-spark/actions/workflows/main.yml">
     <img src="https://github.com/dbt-labs/dbt-spark/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
   </a>
-  <a href="https://github.com/dbt-labs/dbt-spark/actions/workflows/integration.yml">
-    <img src="https://github.com/dbt-labs/dbt-spark/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+  <a href="https://circleci.com/gh/dbt-labs/dbt-spark/?branch=main">
+    <img src="https://circleci.com/gh/dbt-labs/dbt-spark/tree/main.svg?style=shield" alt="Integration Tests Badge"/>
   </a>
 </p>
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.521 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.0 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: ODBC Provides-Extra: PyHive Provides-Extra: session Provides-
-Extra: all
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: ODBC
+Provides-Extra: PyHive Provides-Extra: session Provides-Extra: all
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## in-dbt-spark The `in-dbt-spark` package contains code to
```

### Comparing `in-dbt-spark-1.2.521/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.5.0/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 dbt/adapters/setu/setu_session_request.py
 dbt/adapters/setu/utils.py
 dbt/adapters/spark/__init__.py
 dbt/adapters/spark/__version__.py
 dbt/adapters/spark/column.py
 dbt/adapters/spark/connections.py
 dbt/adapters/spark/impl.py
+dbt/adapters/spark/python_submissions.py
 dbt/adapters/spark/relation.py
 dbt/adapters/spark/session.py
 dbt/adapters/spark/spark_utils.py
 dbt/include/spark/__init__.py
 dbt/include/spark/dbt_project.yml
 dbt/include/spark/profile_template.yml
 dbt/include/spark/macros/adapters.sql
@@ -27,23 +28,29 @@
 dbt/include/spark/macros/apply_retention.sql
 dbt/include/spark/macros/catalog.sql
 dbt/include/spark/macros/materializations/seed.sql
 dbt/include/spark/macros/materializations/snapshot.sql
 dbt/include/spark/macros/materializations/table.sql
 dbt/include/spark/macros/materializations/validate.sql
 dbt/include/spark/macros/materializations/view.sql
+dbt/include/spark/macros/materializations/incremental/column_helpers.sql
 dbt/include/spark/macros/materializations/incremental/incremental.sql
 dbt/include/spark/macros/materializations/incremental/strategies.sql
 dbt/include/spark/macros/utils/any_value.sql
+dbt/include/spark/macros/utils/array_append.sql
+dbt/include/spark/macros/utils/array_concat.sql
+dbt/include/spark/macros/utils/array_construct.sql
 dbt/include/spark/macros/utils/assert_not_null.sql
 dbt/include/spark/macros/utils/bool_or.sql
 dbt/include/spark/macros/utils/concat.sql
 dbt/include/spark/macros/utils/dateadd.sql
 dbt/include/spark/macros/utils/datediff.sql
+dbt/include/spark/macros/utils/escape_single_quotes.sql
 dbt/include/spark/macros/utils/listagg.sql
 dbt/include/spark/macros/utils/split_part.sql
+dbt/include/spark/macros/utils/timestamps.sql
 in_dbt_spark.egg-info/PKG-INFO
 in_dbt_spark.egg-info/SOURCES.txt
 in_dbt_spark.egg-info/dependency_links.txt
 in_dbt_spark.egg-info/not-zip-safe
 in_dbt_spark.egg-info/requires.txt
 in_dbt_spark.egg-info/top_level.txt
```

### Comparing `in-dbt-spark-1.2.521/setup.py` & `in-dbt-spark-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 import os
 import sys
 import re
 
 # require python 3.7 or newer
-if sys.version_info < (3, 8):
+if sys.version_info < (3, 7):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.8 or higher.")
+    print("Please upgrade to Python 3.7 or higher.")
     sys.exit(1)
 
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
@@ -29,15 +29,15 @@
 
 
 # get this package's version from dbt/adapters/<name>/__version__.py
 def _get_plugin_version_dict():
     _version_path = os.path.join(this_directory, "dbt", "adapters", "spark", "__version__.py")
     _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
     _pre = r"""((?P<prekind>a|b|rc)(?P<pre>\d+))?"""
-    _version_pattern = fr"""version\s*=\s*["']{_semver}{_pre}["']"""
+    _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}["']"""
     with open(_version_path) as f:
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
@@ -46,22 +46,22 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.2.521"
+package_version = "1.5.0"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
-    "thrift>=0.11.0,<0.16.0",
+    "thrift>=0.11.0,<0.17.0",
 ]
 session_extras = ["pyspark>=3.0.0,<4.0.0"]
 all_extras = odbc_extras + pyhive_extras + session_extras
 
 setup(
     name=package_name,
     version=package_version,
@@ -87,13 +87,14 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.7",
 )
```

