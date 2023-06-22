# Comparing `tmp/sampy-abm-1.0.1.tar.gz` & `tmp/sampy-abm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampy-abm-1.0.1.tar", last modified: Wed Jun  7 19:13:01 2023, max compression
+gzip compressed data, was "sampy-abm-1.0.2.tar", last modified: Thu Jun 22 17:10:02 2023, max compression
```

## Comparing `sampy-abm-1.0.1.tar` & `sampy-abm-1.0.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.313675 sampy-abm-1.0.1/
--rw-rw-rw-   0        0        0    35149 2023-06-07 19:00:29.000000 sampy-abm-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      823 2023-06-07 19:13:01.313675 sampy-abm-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-06-07 19:10:09.000000 sampy-abm-1.0.1/README.md
--rw-rw-rw-   0        0        0      632 2023-06-07 19:11:38.000000 sampy-abm-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 19:13:01.314674 sampy-abm-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.188030 sampy-abm-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.194051 sampy-abm-1.0.1/src/sampy/
--rw-rw-rw-   0        0        0      106 2023-06-07 18:58:31.000000 sampy-abm-1.0.1/src/sampy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.195064 sampy-abm-1.0.1/src/sampy/addons/
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.202287 sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/
--rw-rw-rw-   0        0        0    32933 2023-06-07 18:58:32.000000 sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/ORM_like_agents.py
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:33.000000 sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/__init__.py
--rw-rw-rw-   0        0        0     7126 2023-06-07 18:58:33.000000 sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py
--rw-rw-rw-   0        0        0    13398 2023-06-07 18:58:33.000000 sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/jit_compiled_function.py
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:32.000000 sampy-abm-1.0.1/src/sampy/addons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.214520 sampy-abm-1.0.1/src/sampy/agent/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:34.000000 sampy-abm-1.0.1/src/sampy/agent/__init__.py
--rw-rw-rw-   0        0        0    11730 2023-06-07 18:58:34.000000 sampy-abm-1.0.1/src/sampy/agent/base.py
--rw-rw-rw-   0        0        0     3860 2023-06-07 18:58:34.000000 sampy-abm-1.0.1/src/sampy/agent/builtin_agent.py
--rw-rw-rw-   0        0        0    24137 2023-06-07 18:58:35.000000 sampy-abm-1.0.1/src/sampy/agent/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    16668 2023-06-07 18:58:35.000000 sampy-abm-1.0.1/src/sampy/agent/mortality.py
--rw-rw-rw-   0        0        0    20506 2023-06-07 18:58:35.000000 sampy-abm-1.0.1/src/sampy/agent/movement.py
--rw-rw-rw-   0        0        0    20600 2023-06-07 18:58:36.000000 sampy-abm-1.0.1/src/sampy/agent/random_walk.py
--rw-rw-rw-   0        0        0    24184 2023-06-07 18:58:36.000000 sampy-abm-1.0.1/src/sampy/agent/reproduction.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.218859 sampy-abm-1.0.1/src/sampy/data_processing/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:36.000000 sampy-abm-1.0.1/src/sampy/data_processing/__init__.py
--rw-rw-rw-   0        0        0     6627 2023-06-07 18:58:37.000000 sampy-abm-1.0.1/src/sampy/data_processing/csv_manager.py
--rw-rw-rw-   0        0        0     1138 2023-06-07 18:58:37.000000 sampy-abm-1.0.1/src/sampy/data_processing/write_file.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.219856 sampy-abm-1.0.1/src/sampy/disease/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:37.000000 sampy-abm-1.0.1/src/sampy/disease/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.229830 sampy-abm-1.0.1/src/sampy/disease/single_species/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:38.000000 sampy-abm-1.0.1/src/sampy/disease/single_species/__init__.py
--rw-rw-rw-   0        0        0     5485 2023-06-07 18:58:38.000000 sampy-abm-1.0.1/src/sampy/disease/single_species/base.py
--rw-rw-rw-   0        0        0     7773 2023-06-07 18:58:38.000000 sampy-abm-1.0.1/src/sampy/disease/single_species/builtin_disease.py
--rw-rw-rw-   0        0        0     3387 2023-06-07 18:58:39.000000 sampy-abm-1.0.1/src/sampy/disease/single_species/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    21124 2023-06-07 18:58:39.000000 sampy-abm-1.0.1/src/sampy/disease/single_species/transition.py
--rw-rw-rw-   0        0        0     7973 2023-06-07 18:58:39.000000 sampy-abm-1.0.1/src/sampy/disease/single_species/transmission.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.238728 sampy-abm-1.0.1/src/sampy/disease/two_species/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:40.000000 sampy-abm-1.0.1/src/sampy/disease/two_species/__init__.py
--rw-rw-rw-   0        0        0     5375 2023-06-07 18:58:40.000000 sampy-abm-1.0.1/src/sampy/disease/two_species/base.py
--rw-rw-rw-   0        0        0    12561 2023-06-07 18:58:40.000000 sampy-abm-1.0.1/src/sampy/disease/two_species/builtin_disease.py
--rw-rw-rw-   0        0        0     7147 2023-06-07 18:58:41.000000 sampy-abm-1.0.1/src/sampy/disease/two_species/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    12671 2023-06-07 18:58:41.000000 sampy-abm-1.0.1/src/sampy/disease/two_species/transition.py
--rw-rw-rw-   0        0        0    11929 2023-06-07 18:58:41.000000 sampy-abm-1.0.1/src/sampy/disease/two_species/transmission.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.252964 sampy-abm-1.0.1/src/sampy/graph/
--rw-rw-rw-   0        0        0       59 2023-06-07 18:58:42.000000 sampy-abm-1.0.1/src/sampy/graph/__init__.py
--rw-rw-rw-   0        0        0     4856 2023-06-07 18:58:42.000000 sampy-abm-1.0.1/src/sampy/graph/builtin_graph.py
--rw-rw-rw-   0        0        0     6844 2023-06-07 18:58:42.000000 sampy-abm-1.0.1/src/sampy/graph/from_files.py
--rw-rw-rw-   0        0        0     7166 2023-06-07 18:58:43.000000 sampy-abm-1.0.1/src/sampy/graph/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    26225 2023-06-07 18:58:43.000000 sampy-abm-1.0.1/src/sampy/graph/misc.py
--rw-rw-rw-   0        0        0    10145 2023-06-07 18:58:43.000000 sampy-abm-1.0.1/src/sampy/graph/spatial_2d.py
--rw-rw-rw-   0        0        0     2869 2023-06-07 18:58:44.000000 sampy-abm-1.0.1/src/sampy/graph/spatial_functions.py
--rw-rw-rw-   0        0        0    12256 2023-06-07 18:58:44.000000 sampy-abm-1.0.1/src/sampy/graph/topology.py
--rw-rw-rw-   0        0        0     7263 2023-06-07 18:58:44.000000 sampy-abm-1.0.1/src/sampy/graph/vertex_attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.263556 sampy-abm-1.0.1/src/sampy/intervention/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:45.000000 sampy-abm-1.0.1/src/sampy/intervention/__init__.py
--rw-rw-rw-   0        0        0      939 2023-06-07 18:58:45.000000 sampy-abm-1.0.1/src/sampy/intervention/built_in_interventions.py
--rw-rw-rw-   0        0        0     2546 2023-06-07 18:58:45.000000 sampy-abm-1.0.1/src/sampy/intervention/culling.py
--rw-rw-rw-   0        0        0     1813 2023-06-07 18:58:46.000000 sampy-abm-1.0.1/src/sampy/intervention/jit_compiled_functions.py
--rw-rw-rw-   0        0        0     2374 2023-06-07 18:58:46.000000 sampy-abm-1.0.1/src/sampy/intervention/sampling.py
--rw-rw-rw-   0        0        0     5010 2023-06-07 18:58:46.000000 sampy-abm-1.0.1/src/sampy/intervention/vaccination.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.267683 sampy-abm-1.0.1/src/sampy/pandas_xs/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:47.000000 sampy-abm-1.0.1/src/sampy/pandas_xs/__init__.py
--rw-rw-rw-   0        0        0      621 2023-06-07 18:58:47.000000 sampy-abm-1.0.1/src/sampy/pandas_xs/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    21328 2023-06-07 18:58:47.000000 sampy-abm-1.0.1/src/sampy/pandas_xs/pandas_xs.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.278308 sampy-abm-1.0.1/src/sampy/spatial/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:48.000000 sampy-abm-1.0.1/src/sampy/spatial/__init__.py
--rw-rw-rw-   0        0        0      797 2023-06-07 18:58:48.000000 sampy-abm-1.0.1/src/sampy/spatial/base_graph_intersection.py
--rw-rw-rw-   0        0        0       21 2023-06-07 18:58:48.000000 sampy-abm-1.0.1/src/sampy/spatial/built_in_graph_intersections.py
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:49.000000 sampy-abm-1.0.1/src/sampy/spatial/builtin_proximity_classes.py
--rw-rw-rw-   0        0        0      800 2023-06-07 18:58:49.000000 sampy-abm-1.0.1/src/sampy/spatial/graph_intersection_geometry.py
--rw-rw-rw-   0        0        0     2381 2023-06-07 18:58:49.000000 sampy-abm-1.0.1/src/sampy/spatial/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    11967 2023-06-07 18:58:50.000000 sampy-abm-1.0.1/src/sampy/spatial/proximity_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.283465 sampy-abm-1.0.1/src/sampy/utils/
--rw-rw-rw-   0        0        0        0 2023-06-07 18:58:50.000000 sampy-abm-1.0.1/src/sampy/utils/__init__.py
--rw-rw-rw-   0        0        0     1939 2023-06-07 18:58:50.000000 sampy-abm-1.0.1/src/sampy/utils/decorators.py
--rw-rw-rw-   0        0        0     2661 2023-06-07 18:58:51.000000 sampy-abm-1.0.1/src/sampy/utils/errors_shortcut.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.303693 sampy-abm-1.0.1/src/sampy_abm.egg-info/
--rw-rw-rw-   0        0        0      823 2023-06-07 19:13:01.000000 sampy-abm-1.0.1/src/sampy_abm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2622 2023-06-07 19:13:01.000000 sampy-abm-1.0.1/src/sampy_abm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 19:13:01.000000 sampy-abm-1.0.1/src/sampy_abm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-07 19:13:01.000000 sampy-abm-1.0.1/src/sampy_abm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 19:13:01.000000 sampy-abm-1.0.1/src/sampy_abm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 19:13:01.311822 sampy-abm-1.0.1/tests/
--rw-rw-rw-   0        0        0    24727 2023-06-07 19:00:28.000000 sampy-abm-1.0.1/tests/test_agents.py
--rw-rw-rw-   0        0        0     3081 2023-06-07 19:00:28.000000 sampy-abm-1.0.1/tests/test_disease_single_species.py
--rw-rw-rw-   0        0        0      639 2023-06-07 19:00:28.000000 sampy-abm-1.0.1/tests/test_disease_two_species.py
--rw-rw-rw-   0        0        0     9469 2023-06-07 19:00:29.000000 sampy-abm-1.0.1/tests/test_graphs.py
--rw-rw-rw-   0        0        0    24740 2023-06-07 19:00:29.000000 sampy-abm-1.0.1/tests/test_pandas_xs.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.535132 sampy-abm-1.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-06-07 19:00:29.000000 sampy-abm-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      823 2023-06-22 17:10:02.535132 sampy-abm-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-06-22 17:08:16.000000 sampy-abm-1.0.2/README.md
+-rw-rw-rw-   0        0        0      632 2023-06-22 17:08:14.000000 sampy-abm-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 17:10:02.536101 sampy-abm-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.393054 sampy-abm-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.412281 sampy-abm-1.0.2/src/sampy/
+-rw-rw-rw-   0        0        0      106 2023-06-22 17:07:25.000000 sampy-abm-1.0.2/src/sampy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.414271 sampy-abm-1.0.2/src/sampy/addons/
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.423384 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/
+-rw-rw-rw-   0        0        0    32933 2023-06-22 17:07:26.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/ORM_like_agents.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:26.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/__init__.py
+-rw-rw-rw-   0        0        0     7126 2023-06-22 17:07:27.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py
+-rw-rw-rw-   0        0        0    13398 2023-06-22 17:07:27.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/jit_compiled_function.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:26.000000 sampy-abm-1.0.2/src/sampy/addons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.440746 sampy-abm-1.0.2/src/sampy/agent/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:27.000000 sampy-abm-1.0.2/src/sampy/agent/__init__.py
+-rw-rw-rw-   0        0        0    11730 2023-06-22 17:07:28.000000 sampy-abm-1.0.2/src/sampy/agent/base.py
+-rw-rw-rw-   0        0        0     3860 2023-06-22 17:07:28.000000 sampy-abm-1.0.2/src/sampy/agent/builtin_agent.py
+-rw-rw-rw-   0        0        0    24137 2023-06-22 17:07:28.000000 sampy-abm-1.0.2/src/sampy/agent/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    16668 2023-06-22 17:07:29.000000 sampy-abm-1.0.2/src/sampy/agent/mortality.py
+-rw-rw-rw-   0        0        0    20506 2023-06-22 17:07:29.000000 sampy-abm-1.0.2/src/sampy/agent/movement.py
+-rw-rw-rw-   0        0        0    20600 2023-06-22 17:07:29.000000 sampy-abm-1.0.2/src/sampy/agent/random_walk.py
+-rw-rw-rw-   0        0        0    24184 2023-06-22 17:07:30.000000 sampy-abm-1.0.2/src/sampy/agent/reproduction.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.445992 sampy-abm-1.0.2/src/sampy/data_processing/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:30.000000 sampy-abm-1.0.2/src/sampy/data_processing/__init__.py
+-rw-rw-rw-   0        0        0     6627 2023-06-22 17:07:30.000000 sampy-abm-1.0.2/src/sampy/data_processing/csv_manager.py
+-rw-rw-rw-   0        0        0     1138 2023-06-22 17:07:31.000000 sampy-abm-1.0.2/src/sampy/data_processing/write_file.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.447607 sampy-abm-1.0.2/src/sampy/disease/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:31.000000 sampy-abm-1.0.2/src/sampy/disease/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.457167 sampy-abm-1.0.2/src/sampy/disease/single_species/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:31.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/__init__.py
+-rw-rw-rw-   0        0        0     5485 2023-06-22 17:07:32.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/base.py
+-rw-rw-rw-   0        0        0     7773 2023-06-22 17:07:32.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/builtin_disease.py
+-rw-rw-rw-   0        0        0     3387 2023-06-22 17:07:32.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    21124 2023-06-22 17:07:33.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/transition.py
+-rw-rw-rw-   0        0        0     7973 2023-06-22 17:07:33.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/transmission.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.465388 sampy-abm-1.0.2/src/sampy/disease/two_species/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:33.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/__init__.py
+-rw-rw-rw-   0        0        0     5375 2023-06-22 17:07:34.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/base.py
+-rw-rw-rw-   0        0        0    12561 2023-06-22 17:07:34.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/builtin_disease.py
+-rw-rw-rw-   0        0        0     7147 2023-06-22 17:07:34.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    12671 2023-06-22 17:07:35.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/transition.py
+-rw-rw-rw-   0        0        0    11929 2023-06-22 17:07:35.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/transmission.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.479984 sampy-abm-1.0.2/src/sampy/graph/
+-rw-rw-rw-   0        0        0       59 2023-06-22 17:07:35.000000 sampy-abm-1.0.2/src/sampy/graph/__init__.py
+-rw-rw-rw-   0        0        0     4856 2023-06-22 17:07:36.000000 sampy-abm-1.0.2/src/sampy/graph/builtin_graph.py
+-rw-rw-rw-   0        0        0     6844 2023-06-22 17:07:36.000000 sampy-abm-1.0.2/src/sampy/graph/from_files.py
+-rw-rw-rw-   0        0        0     7166 2023-06-22 17:07:36.000000 sampy-abm-1.0.2/src/sampy/graph/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    26225 2023-06-22 17:07:37.000000 sampy-abm-1.0.2/src/sampy/graph/misc.py
+-rw-rw-rw-   0        0        0    10145 2023-06-22 17:07:37.000000 sampy-abm-1.0.2/src/sampy/graph/spatial_2d.py
+-rw-rw-rw-   0        0        0     2869 2023-06-22 17:07:37.000000 sampy-abm-1.0.2/src/sampy/graph/spatial_functions.py
+-rw-rw-rw-   0        0        0    12256 2023-06-22 17:07:38.000000 sampy-abm-1.0.2/src/sampy/graph/topology.py
+-rw-rw-rw-   0        0        0     7263 2023-06-22 17:07:38.000000 sampy-abm-1.0.2/src/sampy/graph/vertex_attributes.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.489034 sampy-abm-1.0.2/src/sampy/intervention/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:38.000000 sampy-abm-1.0.2/src/sampy/intervention/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-06-22 17:07:39.000000 sampy-abm-1.0.2/src/sampy/intervention/built_in_interventions.py
+-rw-rw-rw-   0        0        0     2543 2023-06-22 17:07:39.000000 sampy-abm-1.0.2/src/sampy/intervention/culling.py
+-rw-rw-rw-   0        0        0     1813 2023-06-22 17:07:39.000000 sampy-abm-1.0.2/src/sampy/intervention/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0     2374 2023-06-22 17:07:40.000000 sampy-abm-1.0.2/src/sampy/intervention/sampling.py
+-rw-rw-rw-   0        0        0     5007 2023-06-22 17:07:40.000000 sampy-abm-1.0.2/src/sampy/intervention/vaccination.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.493041 sampy-abm-1.0.2/src/sampy/pandas_xs/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:40.000000 sampy-abm-1.0.2/src/sampy/pandas_xs/__init__.py
+-rw-rw-rw-   0        0        0      621 2023-06-22 17:07:41.000000 sampy-abm-1.0.2/src/sampy/pandas_xs/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    21328 2023-06-22 17:07:41.000000 sampy-abm-1.0.2/src/sampy/pandas_xs/pandas_xs.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.502142 sampy-abm-1.0.2/src/sampy/spatial/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:41.000000 sampy-abm-1.0.2/src/sampy/spatial/__init__.py
+-rw-rw-rw-   0        0        0      797 2023-06-22 17:07:42.000000 sampy-abm-1.0.2/src/sampy/spatial/base_graph_intersection.py
+-rw-rw-rw-   0        0        0       21 2023-06-22 17:07:42.000000 sampy-abm-1.0.2/src/sampy/spatial/built_in_graph_intersections.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:42.000000 sampy-abm-1.0.2/src/sampy/spatial/builtin_proximity_classes.py
+-rw-rw-rw-   0        0        0      800 2023-06-22 17:07:43.000000 sampy-abm-1.0.2/src/sampy/spatial/graph_intersection_geometry.py
+-rw-rw-rw-   0        0        0     2381 2023-06-22 17:07:43.000000 sampy-abm-1.0.2/src/sampy/spatial/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    11967 2023-06-22 17:07:43.000000 sampy-abm-1.0.2/src/sampy/spatial/proximity_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.505982 sampy-abm-1.0.2/src/sampy/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:07:44.000000 sampy-abm-1.0.2/src/sampy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1939 2023-06-22 17:07:44.000000 sampy-abm-1.0.2/src/sampy/utils/decorators.py
+-rw-rw-rw-   0        0        0     2661 2023-06-22 17:07:44.000000 sampy-abm-1.0.2/src/sampy/utils/errors_shortcut.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.525078 sampy-abm-1.0.2/src/sampy_abm.egg-info/
+-rw-rw-rw-   0        0        0      823 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2622 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.532980 sampy-abm-1.0.2/tests/
+-rw-rw-rw-   0        0        0    24727 2023-06-22 17:07:19.000000 sampy-abm-1.0.2/tests/test_agents.py
+-rw-rw-rw-   0        0        0     3081 2023-06-22 17:07:19.000000 sampy-abm-1.0.2/tests/test_disease_single_species.py
+-rw-rw-rw-   0        0        0      639 2023-06-22 17:07:20.000000 sampy-abm-1.0.2/tests/test_disease_two_species.py
+-rw-rw-rw-   0        0        0     9469 2023-06-22 17:07:20.000000 sampy-abm-1.0.2/tests/test_graphs.py
+-rw-rw-rw-   0        0        0    24740 2023-06-22 17:07:20.000000 sampy-abm-1.0.2/tests/test_pandas_xs.py
```

### Comparing `sampy-abm-1.0.1/LICENSE` & `sampy-abm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/PKG-INFO` & `sampy-abm-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampy-abm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for ABM development in epidemiology.
 Author-email: Francois Viard <sampy.project@gmail.com>
 Project-URL: Homepage, https://github.com/sampy-project/sampy-main
 Project-URL: Bug Tracker, https://github.com/sampy-project/sampy-main/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampy-abm-1.0.1/pyproject.toml` & `sampy-abm-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sampy-abm"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name = "Francois Viard", email = "sampy.project@gmail.com" },
 ]
 description = "Library for ABM development in epidemiology."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/ORM_like_agents.py` & `sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/ORM_like_agents.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py` & `sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/addons/ORM_related_addons/jit_compiled_function.py` & `sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/jit_compiled_function.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/base.py` & `sampy-abm-1.0.2/src/sampy/agent/base.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/builtin_agent.py` & `sampy-abm-1.0.2/src/sampy/agent/builtin_agent.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/agent/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/mortality.py` & `sampy-abm-1.0.2/src/sampy/agent/mortality.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/movement.py` & `sampy-abm-1.0.2/src/sampy/agent/movement.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/random_walk.py` & `sampy-abm-1.0.2/src/sampy/agent/random_walk.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/agent/reproduction.py` & `sampy-abm-1.0.2/src/sampy/agent/reproduction.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/data_processing/csv_manager.py` & `sampy-abm-1.0.2/src/sampy/data_processing/csv_manager.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/data_processing/write_file.py` & `sampy-abm-1.0.2/src/sampy/data_processing/write_file.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/single_species/base.py` & `sampy-abm-1.0.2/src/sampy/disease/single_species/base.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/single_species/builtin_disease.py` & `sampy-abm-1.0.2/src/sampy/disease/single_species/builtin_disease.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/single_species/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/disease/single_species/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/single_species/transition.py` & `sampy-abm-1.0.2/src/sampy/disease/single_species/transition.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/single_species/transmission.py` & `sampy-abm-1.0.2/src/sampy/disease/single_species/transmission.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/two_species/base.py` & `sampy-abm-1.0.2/src/sampy/disease/two_species/base.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/two_species/builtin_disease.py` & `sampy-abm-1.0.2/src/sampy/disease/two_species/builtin_disease.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/two_species/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/disease/two_species/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/two_species/transition.py` & `sampy-abm-1.0.2/src/sampy/disease/two_species/transition.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/disease/two_species/transmission.py` & `sampy-abm-1.0.2/src/sampy/disease/two_species/transmission.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/builtin_graph.py` & `sampy-abm-1.0.2/src/sampy/graph/builtin_graph.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/from_files.py` & `sampy-abm-1.0.2/src/sampy/graph/from_files.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/graph/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/misc.py` & `sampy-abm-1.0.2/src/sampy/graph/misc.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/spatial_2d.py` & `sampy-abm-1.0.2/src/sampy/graph/spatial_2d.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/spatial_functions.py` & `sampy-abm-1.0.2/src/sampy/graph/spatial_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/topology.py` & `sampy-abm-1.0.2/src/sampy/graph/topology.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/graph/vertex_attributes.py` & `sampy-abm-1.0.2/src/sampy/graph/vertex_attributes.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/intervention/built_in_interventions.py` & `sampy-abm-1.0.2/src/sampy/intervention/built_in_interventions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/intervention/culling.py` & `sampy-abm-1.0.2/src/sampy/intervention/culling.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         values is the culling level on each cell.
 
         :param graph: graph object on which the culling is applied
         :param dict_vertex_id_to_level: dictionnary-like object with culling level
         :param condition: optional, 1D array of bool, default None.
         :param position_attribute: optional, string, default 'position'.
         """
-        array_cul_level = np.full((graph.number_vertices,), 0., dtype=np.float)
+        array_cul_level = np.full((graph.number_vertices,), 0., dtype=float)
         for id_vertex, level in dict_vertex_id_to_level.items():
             array_cul_level[graph.dict_cell_id_to_ind[id_vertex]] = level
         self.apply_culling_from_array(array_cul_level, condition=condition, position_attribute=position_attribute)
```

### Comparing `sampy-abm-1.0.1/src/sampy/intervention/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/intervention/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/intervention/sampling.py` & `sampy-abm-1.0.2/src/sampy/intervention/sampling.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/intervention/vaccination.py` & `sampy-abm-1.0.2/src/sampy/intervention/vaccination.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,12 +76,12 @@
         values is the vaccination level on each cell.
 
         :param graph: graph object on which the vaccine is applied
         :param dict_vertex_id_to_level: dictionnary-like object with vaccine level
         :param condition: optional, 1D array of bool, default None.
         :param position_attribute: optional, string, default 'position'.
         """
-        array_vac_level = np.full((graph.number_vertices,), 0., dtype=np.float)
+        array_vac_level = np.full((graph.number_vertices,), 0., dtype=float)
         for id_vertex, level in dict_vertex_id_to_level.items():
             array_vac_level[graph.dict_cell_id_to_ind[id_vertex]] = level
 
         self.apply_vaccine_from_array(array_vac_level, condition=condition, position_attribute=position_attribute)
```

### Comparing `sampy-abm-1.0.1/src/sampy/pandas_xs/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/pandas_xs/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/pandas_xs/pandas_xs.py` & `sampy-abm-1.0.2/src/sampy/pandas_xs/pandas_xs.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/spatial/base_graph_intersection.py` & `sampy-abm-1.0.2/src/sampy/spatial/base_graph_intersection.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/spatial/graph_intersection_geometry.py` & `sampy-abm-1.0.2/src/sampy/spatial/graph_intersection_geometry.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/spatial/jit_compiled_functions.py` & `sampy-abm-1.0.2/src/sampy/spatial/jit_compiled_functions.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/spatial/proximity_3d.py` & `sampy-abm-1.0.2/src/sampy/spatial/proximity_3d.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/utils/decorators.py` & `sampy-abm-1.0.2/src/sampy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy/utils/errors_shortcut.py` & `sampy-abm-1.0.2/src/sampy/utils/errors_shortcut.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/src/sampy_abm.egg-info/PKG-INFO` & `sampy-abm-1.0.2/src/sampy_abm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampy-abm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for ABM development in epidemiology.
 Author-email: Francois Viard <sampy.project@gmail.com>
 Project-URL: Homepage, https://github.com/sampy-project/sampy-main
 Project-URL: Bug Tracker, https://github.com/sampy-project/sampy-main/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampy-abm-1.0.1/src/sampy_abm.egg-info/SOURCES.txt` & `sampy-abm-1.0.2/src/sampy_abm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/tests/test_agents.py` & `sampy-abm-1.0.2/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/tests/test_disease_single_species.py` & `sampy-abm-1.0.2/tests/test_disease_single_species.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/tests/test_disease_two_species.py` & `sampy-abm-1.0.2/tests/test_disease_two_species.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/tests/test_graphs.py` & `sampy-abm-1.0.2/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.1/tests/test_pandas_xs.py` & `sampy-abm-1.0.2/tests/test_pandas_xs.py`

 * *Files identical despite different names*

