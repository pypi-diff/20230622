# Comparing `tmp/djraphql-0.2.8.tar.gz` & `tmp/djraphql-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djraphql-0.2.8.tar", last modified: Thu Dec  1 22:01:46 2022, max compression
+gzip compressed data, was "djraphql-0.2.9.tar", last modified: Mon Dec  5 18:33:23 2022, max compression
```

## Comparing `djraphql-0.2.8.tar` & `djraphql-0.2.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.563000 djraphql-0.2.8/
--rw-r--r--   0 joel       (503) staff       (20)     1090 2022-08-11 22:18:17.000000 djraphql-0.2.8/LICENSE
--rw-r--r--   0 joel       (503) staff       (20)       50 2022-08-11 22:18:17.000000 djraphql-0.2.8/MANIFEST.in
--rw-r--r--   0 joel       (503) staff       (20)     2591 2022-12-01 22:01:46.562833 djraphql-0.2.8/PKG-INFO
--rw-r--r--   0 joel       (503) staff       (20)     2166 2022-08-11 22:18:17.000000 djraphql-0.2.8/README.md
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.553448 djraphql-0.2.8/djraphql/
--rw-r--r--   0 joel       (503) staff       (20)      349 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     2695 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/access_permissions.py
--rw-r--r--   0 joel       (503) staff       (20)     1191 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/django_models.py
--rw-r--r--   0 joel       (503) staff       (20)     5455 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/entities.py
--rw-r--r--   0 joel       (503) staff       (20)     1909 2022-08-12 15:38:22.000000 djraphql-0.2.8/djraphql/fields.py
--rw-r--r--   0 joel       (503) staff       (20)      151 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/filters.py
--rw-r--r--   0 joel       (503) staff       (20)      893 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schema_builder.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.554775 djraphql-0.2.8/djraphql/schemas/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     2242 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/abstract_type_builder.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.555331 djraphql-0.2.8/djraphql/schemas/default/
--rw-r--r--   0 joel       (503) staff       (20)     6127 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     1900 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/mappings.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.556686 djraphql-0.2.8/djraphql/schemas/default/resolvers/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     8887 2022-12-01 22:00:39.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/aggregate.py
--rw-r--r--   0 joel       (503) staff       (20)      509 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/by_pk.py
--rw-r--r--   0 joel       (503) staff       (20)     1524 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/delete.py
--rw-r--r--   0 joel       (503) staff       (20)      232 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/field.py
--rw-r--r--   0 joel       (503) staff       (20)      151 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/group_by.py
--rw-r--r--   0 joel       (503) staff       (20)     8087 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/insert.py
--rw-r--r--   0 joel       (503) staff       (20)     3220 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/list.py
--rw-r--r--   0 joel       (503) staff       (20)    11618 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/resolvers/update.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.556828 djraphql-0.2.8/djraphql/schemas/default/types/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/__init__.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.557297 djraphql-0.2.8/djraphql/schemas/default/types/mutations/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/mutations/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     1782 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/mutations/delete.py
--rw-r--r--   0 joel       (503) staff       (20)     3539 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/mutations/insert.py
--rw-r--r--   0 joel       (503) staff       (20)     3534 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/mutations/update.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.557853 djraphql-0.2.8/djraphql/schemas/default/types/queries/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/queries/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     1959 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/queries/aggregate.py
--rw-r--r--   0 joel       (503) staff       (20)     1363 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/queries/by_pk.py
--rw-r--r--   0 joel       (503) staff       (20)     1585 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/queries/many.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.560595 djraphql-0.2.8/djraphql/schemas/default/types/shared/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     4636 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/aggregate_basic.py
--rw-r--r--   0 joel       (503) staff       (20)     1630 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/aggregate_group_by.py
--rw-r--r--   0 joel       (503) staff       (20)     2064 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/aggregate_result.py
--rw-r--r--   0 joel       (503) staff       (20)     4735 2022-08-12 15:38:22.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/basic.py
--rw-r--r--   0 joel       (503) staff       (20)     1644 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/enum.py
--rw-r--r--   0 joel       (503) staff       (20)     3784 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/insert_input_type.py
--rw-r--r--   0 joel       (503) staff       (20)     1085 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/list_update_input_type.py
--rw-r--r--   0 joel       (503) staff       (20)      835 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/nested_item_insert_input_type.py
--rw-r--r--   0 joel       (503) staff       (20)     1191 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/nested_item_update_input_type.py
--rw-r--r--   0 joel       (503) staff       (20)     1239 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/order_clause.py
--rw-r--r--   0 joel       (503) staff       (20)     1084 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/pk_input.py
--rw-r--r--   0 joel       (503) staff       (20)      504 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/tag_to_pk.py
--rw-r--r--   0 joel       (503) staff       (20)     4366 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/update_input_type.py
--rw-r--r--   0 joel       (503) staff       (20)     3813 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/where_clause.py
--rw-r--r--   0 joel       (503) staff       (20)     1447 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/types/shared/where_predicate.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.561360 djraphql-0.2.8/djraphql/schemas/default/util/
--rw-r--r--   0 joel       (503) staff       (20)      903 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     5310 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/arguments.py
--rw-r--r--   0 joel       (503) staff       (20)     4079 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/queryset_optimizer.py
--rw-r--r--   0 joel       (503) staff       (20)     3823 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/validation.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.562255 djraphql-0.2.8/djraphql/schemas/default/util/visitors/
--rw-r--r--   0 joel       (503) staff       (20)      712 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/visitors/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)     5807 2022-08-19 16:38:45.000000 djraphql-0.2.8/djraphql/schemas/default/util/visitors/query_fields_visitor.py
--rw-r--r--   0 joel       (503) staff       (20)     7306 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/visitors/queryset_optimization_visitor.py
--rw-r--r--   0 joel       (503) staff       (20)      967 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/schemas/default/util/visitors/read_permissions_check_visitor.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.562573 djraphql-0.2.8/djraphql/tests/
--rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/tests/__init__.py
--rw-r--r--   0 joel       (503) staff       (20)      572 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/tests/test_visitors.py
--rw-r--r--   0 joel       (503) staff       (20)     8996 2022-08-11 22:18:17.000000 djraphql-0.2.8/djraphql/type_registry.py
-drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-01 22:01:46.554497 djraphql-0.2.8/djraphql.egg-info/
--rw-r--r--   0 joel       (503) staff       (20)     2591 2022-12-01 22:01:46.000000 djraphql-0.2.8/djraphql.egg-info/PKG-INFO
--rw-r--r--   0 joel       (503) staff       (20)     2795 2022-12-01 22:01:46.000000 djraphql-0.2.8/djraphql.egg-info/SOURCES.txt
--rw-r--r--   0 joel       (503) staff       (20)        1 2022-12-01 22:01:46.000000 djraphql-0.2.8/djraphql.egg-info/dependency_links.txt
--rw-r--r--   0 joel       (503) staff       (20)       20 2022-12-01 22:01:46.000000 djraphql-0.2.8/djraphql.egg-info/requires.txt
--rw-r--r--   0 joel       (503) staff       (20)       26 2022-12-01 22:01:46.000000 djraphql-0.2.8/djraphql.egg-info/top_level.txt
--rw-r--r--   0 joel       (503) staff       (20)       38 2022-12-01 22:01:46.563048 djraphql-0.2.8/setup.cfg
--rw-r--r--   0 joel       (503) staff       (20)      795 2022-12-01 22:01:34.000000 djraphql-0.2.8/setup.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.190304 djraphql-0.2.9/
+-rw-r--r--   0 joel       (503) staff       (20)     1090 2022-08-11 22:18:17.000000 djraphql-0.2.9/LICENSE
+-rw-r--r--   0 joel       (503) staff       (20)       50 2022-08-11 22:18:17.000000 djraphql-0.2.9/MANIFEST.in
+-rw-r--r--   0 joel       (503) staff       (20)     2591 2022-12-05 18:33:23.190154 djraphql-0.2.9/PKG-INFO
+-rw-r--r--   0 joel       (503) staff       (20)     2166 2022-08-11 22:18:17.000000 djraphql-0.2.9/README.md
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.181748 djraphql-0.2.9/djraphql/
+-rw-r--r--   0 joel       (503) staff       (20)      349 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     2695 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/access_permissions.py
+-rw-r--r--   0 joel       (503) staff       (20)     1191 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/django_models.py
+-rw-r--r--   0 joel       (503) staff       (20)     5455 2022-12-02 23:27:56.000000 djraphql-0.2.9/djraphql/entities.py
+-rw-r--r--   0 joel       (503) staff       (20)     1909 2022-12-02 23:27:56.000000 djraphql-0.2.9/djraphql/fields.py
+-rw-r--r--   0 joel       (503) staff       (20)      151 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/filters.py
+-rw-r--r--   0 joel       (503) staff       (20)      893 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schema_builder.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.182649 djraphql-0.2.9/djraphql/schemas/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     2242 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/abstract_type_builder.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.182973 djraphql-0.2.9/djraphql/schemas/default/
+-rw-r--r--   0 joel       (503) staff       (20)     6127 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     1900 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/mappings.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.184301 djraphql-0.2.9/djraphql/schemas/default/resolvers/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     8887 2022-12-02 23:27:56.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/aggregate.py
+-rw-r--r--   0 joel       (503) staff       (20)      509 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/by_pk.py
+-rw-r--r--   0 joel       (503) staff       (20)     1524 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/delete.py
+-rw-r--r--   0 joel       (503) staff       (20)      232 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/field.py
+-rw-r--r--   0 joel       (503) staff       (20)      151 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/group_by.py
+-rw-r--r--   0 joel       (503) staff       (20)     8087 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/insert.py
+-rw-r--r--   0 joel       (503) staff       (20)     3220 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/list.py
+-rw-r--r--   0 joel       (503) staff       (20)    11618 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/resolvers/update.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.184460 djraphql-0.2.9/djraphql/schemas/default/types/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/__init__.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.185025 djraphql-0.2.9/djraphql/schemas/default/types/mutations/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/mutations/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     1782 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/mutations/delete.py
+-rw-r--r--   0 joel       (503) staff       (20)     3539 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/mutations/insert.py
+-rw-r--r--   0 joel       (503) staff       (20)     3534 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/mutations/update.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.185532 djraphql-0.2.9/djraphql/schemas/default/types/queries/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/queries/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     1959 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/queries/aggregate.py
+-rw-r--r--   0 joel       (503) staff       (20)     1363 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/queries/by_pk.py
+-rw-r--r--   0 joel       (503) staff       (20)     1585 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/queries/many.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.187975 djraphql-0.2.9/djraphql/schemas/default/types/shared/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     4636 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/aggregate_basic.py
+-rw-r--r--   0 joel       (503) staff       (20)     1630 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/aggregate_group_by.py
+-rw-r--r--   0 joel       (503) staff       (20)     2064 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/aggregate_result.py
+-rw-r--r--   0 joel       (503) staff       (20)     4735 2022-12-02 23:27:56.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/basic.py
+-rw-r--r--   0 joel       (503) staff       (20)     1644 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/enum.py
+-rw-r--r--   0 joel       (503) staff       (20)     3784 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/insert_input_type.py
+-rw-r--r--   0 joel       (503) staff       (20)     1085 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/list_update_input_type.py
+-rw-r--r--   0 joel       (503) staff       (20)      835 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/nested_item_insert_input_type.py
+-rw-r--r--   0 joel       (503) staff       (20)     1191 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/nested_item_update_input_type.py
+-rw-r--r--   0 joel       (503) staff       (20)     1239 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/order_clause.py
+-rw-r--r--   0 joel       (503) staff       (20)     1084 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/pk_input.py
+-rw-r--r--   0 joel       (503) staff       (20)      504 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/tag_to_pk.py
+-rw-r--r--   0 joel       (503) staff       (20)     4366 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/update_input_type.py
+-rw-r--r--   0 joel       (503) staff       (20)     3813 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/where_clause.py
+-rw-r--r--   0 joel       (503) staff       (20)     1447 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/types/shared/where_predicate.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.188595 djraphql-0.2.9/djraphql/schemas/default/util/
+-rw-r--r--   0 joel       (503) staff       (20)      903 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/util/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     5310 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/util/arguments.py
+-rw-r--r--   0 joel       (503) staff       (20)     4079 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/util/queryset_optimizer.py
+-rw-r--r--   0 joel       (503) staff       (20)     4538 2022-12-05 18:32:53.000000 djraphql-0.2.9/djraphql/schemas/default/util/validation.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.189494 djraphql-0.2.9/djraphql/schemas/default/util/visitors/
+-rw-r--r--   0 joel       (503) staff       (20)      712 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/util/visitors/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)     5807 2022-12-02 23:27:56.000000 djraphql-0.2.9/djraphql/schemas/default/util/visitors/query_fields_visitor.py
+-rw-r--r--   0 joel       (503) staff       (20)     7306 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/util/visitors/queryset_optimization_visitor.py
+-rw-r--r--   0 joel       (503) staff       (20)      967 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/schemas/default/util/visitors/read_permissions_check_visitor.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.189904 djraphql-0.2.9/djraphql/tests/
+-rw-r--r--   0 joel       (503) staff       (20)        0 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/tests/__init__.py
+-rw-r--r--   0 joel       (503) staff       (20)      572 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/tests/test_visitors.py
+-rw-r--r--   0 joel       (503) staff       (20)     8996 2022-08-11 22:18:17.000000 djraphql-0.2.9/djraphql/type_registry.py
+drwxr-xr-x   0 joel       (503) staff       (20)        0 2022-12-05 18:33:23.182439 djraphql-0.2.9/djraphql.egg-info/
+-rw-r--r--   0 joel       (503) staff       (20)     2591 2022-12-05 18:33:23.000000 djraphql-0.2.9/djraphql.egg-info/PKG-INFO
+-rw-r--r--   0 joel       (503) staff       (20)     2795 2022-12-05 18:33:23.000000 djraphql-0.2.9/djraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 joel       (503) staff       (20)        1 2022-12-05 18:33:23.000000 djraphql-0.2.9/djraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 joel       (503) staff       (20)       20 2022-12-05 18:33:23.000000 djraphql-0.2.9/djraphql.egg-info/requires.txt
+-rw-r--r--   0 joel       (503) staff       (20)       26 2022-12-05 18:33:23.000000 djraphql-0.2.9/djraphql.egg-info/top_level.txt
+-rw-r--r--   0 joel       (503) staff       (20)       38 2022-12-05 18:33:23.190361 djraphql-0.2.9/setup.cfg
+-rw-r--r--   0 joel       (503) staff       (20)      795 2022-12-05 18:32:59.000000 djraphql-0.2.9/setup.py
```

### Comparing `djraphql-0.2.8/LICENSE` & `djraphql-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/PKG-INFO` & `djraphql-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djraphql
-Version: 0.2.8
+Version: 0.2.9
 Summary: DjraphQL builds a flexible & performant GraphQL schema by examining your Django models.
 Home-page: https://github.com/Radico/djraphql
 Author: Joel Gardner
 Author-email: joel@simondata.com
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `djraphql-0.2.8/README.md` & `djraphql-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/access_permissions.py` & `djraphql-0.2.9/djraphql/access_permissions.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/django_models.py` & `djraphql-0.2.9/djraphql/django_models.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/entities.py` & `djraphql-0.2.9/djraphql/entities.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/fields.py` & `djraphql-0.2.9/djraphql/fields.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schema_builder.py` & `djraphql-0.2.9/djraphql/schema_builder.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/abstract_type_builder.py` & `djraphql-0.2.9/djraphql/schemas/abstract_type_builder.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/__init__.py` & `djraphql-0.2.9/djraphql/schemas/default/__init__.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/mappings.py` & `djraphql-0.2.9/djraphql/schemas/default/mappings.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/resolvers/aggregate.py` & `djraphql-0.2.9/djraphql/schemas/default/resolvers/aggregate.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/resolvers/delete.py` & `djraphql-0.2.9/djraphql/schemas/default/resolvers/delete.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/resolvers/insert.py` & `djraphql-0.2.9/djraphql/schemas/default/resolvers/insert.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/resolvers/list.py` & `djraphql-0.2.9/djraphql/schemas/default/resolvers/list.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/resolvers/update.py` & `djraphql-0.2.9/djraphql/schemas/default/resolvers/update.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/mutations/delete.py` & `djraphql-0.2.9/djraphql/schemas/default/types/mutations/delete.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/mutations/insert.py` & `djraphql-0.2.9/djraphql/schemas/default/types/mutations/insert.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/mutations/update.py` & `djraphql-0.2.9/djraphql/schemas/default/types/mutations/update.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/queries/aggregate.py` & `djraphql-0.2.9/djraphql/schemas/default/types/queries/aggregate.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/queries/by_pk.py` & `djraphql-0.2.9/djraphql/schemas/default/types/queries/by_pk.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/queries/many.py` & `djraphql-0.2.9/djraphql/schemas/default/types/queries/many.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/aggregate_basic.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/aggregate_basic.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/aggregate_group_by.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/aggregate_group_by.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/aggregate_result.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/aggregate_result.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/basic.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/basic.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/enum.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/enum.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/insert_input_type.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/insert_input_type.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/list_update_input_type.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/list_update_input_type.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/nested_item_insert_input_type.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/nested_item_insert_input_type.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/nested_item_update_input_type.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/nested_item_update_input_type.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/order_clause.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/order_clause.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/pk_input.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/pk_input.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/update_input_type.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/update_input_type.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/where_clause.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/where_clause.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/types/shared/where_predicate.py` & `djraphql-0.2.9/djraphql/schemas/default/types/shared/where_predicate.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/__init__.py` & `djraphql-0.2.9/djraphql/schemas/default/util/__init__.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/arguments.py` & `djraphql-0.2.9/djraphql/schemas/default/util/arguments.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/queryset_optimizer.py` & `djraphql-0.2.9/djraphql/schemas/default/util/queryset_optimizer.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/validation.py` & `djraphql-0.2.9/djraphql/schemas/default/util/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,63 @@
 from functools import reduce
+from enum import Enum
 from graphene.utils.str_converters import to_camel_case
 
 
 class FatalValidationError(Exception):
     pass
 
 
 class ValidatableInput:
     def __init__(self, raw_input, root_model_class, is_insert=True):
         self._raw_input = raw_input
         self._root_model_class = root_model_class
         self._is_insert = is_insert
 
     def to_value(self, camel_case_keys=False, lift_lists=True):
+        # Shallow copy so we don't mutate self._raw_input
+        # Note that using deepcopy here resulted in a weird
+        # "list is not callable" error deep within the deepcopy code...
+        value = self._raw_input.copy()
 
-        value = self._raw_input
         if lift_lists:
             # The input format for inserts and updates is slightly different:
             # Update input objects go one level deeper -- via an "items" key -- to get
             # the actual item being updated. So to lift the *-to-many fields up,
             # we need to account for that. This extract_list helper performs the
             # correct traversal based on the path variable.
             path = [] if self._is_insert else ["items"]
             extract_list = lambda items: reduce(lambda a, b: a[b], path, items)
             value = self._lift_lists_to_related_key(
                 value, self._root_model_class, extract_list
             )
 
+        value = self._convert_enum_values_to_strings(value)
+
         if camel_case_keys:
             value = self._camel_case_keys(value)
 
         return value
 
     @classmethod
+    def _convert_enum_values_to_strings(cls, value):
+        if isinstance(value, Enum):
+            return value.name
+
+        if isinstance(value, dict):
+            return {
+                key: cls._convert_enum_values_to_strings(value[key]) for key in value
+            }
+
+        if isinstance(value, list):
+            return [cls._convert_enum_values_to_strings(item) for item in value]
+
+        return value
+
+    @classmethod
     def _camel_case_keys(cls, value):
         if not value or not isinstance(value, dict):
             return value
 
         result = {}
         for k in value:
             result[to_camel_case(k)] = cls._camel_case_keys(value[k])
```

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/visitors/__init__.py` & `djraphql-0.2.9/djraphql/schemas/default/util/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/visitors/query_fields_visitor.py` & `djraphql-0.2.9/djraphql/schemas/default/util/visitors/query_fields_visitor.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/visitors/queryset_optimization_visitor.py` & `djraphql-0.2.9/djraphql/schemas/default/util/visitors/queryset_optimization_visitor.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/schemas/default/util/visitors/read_permissions_check_visitor.py` & `djraphql-0.2.9/djraphql/schemas/default/util/visitors/read_permissions_check_visitor.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/tests/test_visitors.py` & `djraphql-0.2.9/djraphql/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql/type_registry.py` & `djraphql-0.2.9/djraphql/type_registry.py`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/djraphql.egg-info/PKG-INFO` & `djraphql-0.2.9/djraphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djraphql
-Version: 0.2.8
+Version: 0.2.9
 Summary: DjraphQL builds a flexible & performant GraphQL schema by examining your Django models.
 Home-page: https://github.com/Radico/djraphql
 Author: Joel Gardner
 Author-email: joel@simondata.com
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `djraphql-0.2.8/djraphql.egg-info/SOURCES.txt` & `djraphql-0.2.9/djraphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djraphql-0.2.8/setup.py` & `djraphql-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 setuptools.setup(
     name="djraphql",
     version=VERSION,
     author="Joel Gardner",
     author_email="joel@simondata.com",
     description="DjraphQL builds a flexible & performant GraphQL schema by examining your Django models.",
```

