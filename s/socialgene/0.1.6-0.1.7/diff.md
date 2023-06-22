# Comparing `tmp/socialgene-0.1.6.tar.gz` & `tmp/socialgene-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialgene-0.1.6.tar", last modified: Wed Jun 21 17:01:42 2023, max compression
+gzip compressed data, was "socialgene-0.1.7.tar", last modified: Thu Jun 22 16:30:05 2023, max compression
```

## Comparing `socialgene-0.1.6.tar` & `socialgene-0.1.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.784445 socialgene-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 17:01:34.000000 socialgene-0.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-21 17:01:42.784445 socialgene-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-21 17:01:34.000000 socialgene-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-21 17:01:34.000000 socialgene-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-21 17:01:42.784445 socialgene-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-21 17:01:34.000000 socialgene-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.776445 socialgene-0.1.6/socialgene/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.776445 socialgene-0.1.6/socialgene/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/base/compare_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/base/molbio.py
--rw-r--r--   0 runner    (1001) docker     (123)    26075 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/base/socialgene.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/clean_hmms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/create_neo4j_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/export_neo4j_header_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/export_protein_loci_assembly_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/parameter_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/parse_ncbi_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/parse_ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/process_domtblout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/cli/socialgene_hmm_tsv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/clustermap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/clustermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/clustermap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/common_parameters.env
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/data/biosample_attributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/findmybgc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/findmybgc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/findmybgc/findmybgc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/hashing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/hashing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/hashing/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/hmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/hmm/hmmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/hmm/hmminfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/mmseqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/mmseqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/mmseqs/create_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/mmseqs/index_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/mmseqs/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/admin_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/ingest_from_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/queries.cypher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/neo4j/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/schema/define_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/schema/define_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/schema/define_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/schema/node_relationship_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/schema/socialgene_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.780445 socialgene-0.1.6/socialgene/neo4j/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/search/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/neo4j/single_protein_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.784445 socialgene-0.1.6/socialgene/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/datasets_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/hmmer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/hmmmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/ncbi_feature_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/parsers/sequence_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.784445 socialgene-0.1.6/socialgene/scoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/scoring/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.784445 socialgene-0.1.6/socialgene/taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/taxonomy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.784445 socialgene-0.1.6/socialgene/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/chunker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/get_ncbi_biosample_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/goterms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/ncbi_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/nextflow_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/np_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/prep_ncbi_biosample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/run_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/simple_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/untargz.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-21 17:01:34.000000 socialgene-0.1.6/socialgene/utils/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:42.776445 socialgene-0.1.6/socialgene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-21 17:01:42.000000 socialgene-0.1.6/socialgene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-21 17:01:42.000000 socialgene-0.1.6/socialgene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:01:42.000000 socialgene-0.1.6/socialgene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 17:01:42.000000 socialgene-0.1.6/socialgene.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 17:01:42.000000 socialgene-0.1.6/socialgene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 17:01:42.000000 socialgene-0.1.6/socialgene.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.554987 socialgene-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 16:29:57.000000 socialgene-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 16:30:05.554987 socialgene-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-22 16:29:57.000000 socialgene-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-22 16:29:57.000000 socialgene-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-22 16:30:05.554987 socialgene-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-22 16:29:57.000000 socialgene-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.542986 socialgene-0.1.7/socialgene/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/base/compare_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/base/molbio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26075 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/base/socialgene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/clean_hmms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/create_neo4j_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/export_neo4j_header_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/export_protein_loci_assembly_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/parameter_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/parse_ncbi_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/parse_ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/process_domtblout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/cli/socialgene_hmm_tsv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/clustermap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/clustermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/clustermap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/common_parameters.env
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/data/biosample_attributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/findmybgc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/findmybgc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/findmybgc/findmybgc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/hashing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/hashing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/hashing/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/hmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/hmm/hmmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/hmm/hmminfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene/mmseqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/mmseqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/mmseqs/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/mmseqs/index_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/mmseqs/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/admin_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/ingest_from_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/queries.cypher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/neo4j/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/schema/define_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/schema/define_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/schema/define_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/schema/node_relationship_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/schema/socialgene_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/neo4j/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/search/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/neo4j/single_protein_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/datasets_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/hmmer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/hmmmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/ncbi_feature_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/parsers/sequence_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/scoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/scoring/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/taxonomy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.550986 socialgene-0.1.7/socialgene/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/chunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/get_ncbi_biosample_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/goterms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/ncbi_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/nextflow_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/np_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/prep_ncbi_biosample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/run_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/simple_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/untargz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 16:29:57.000000 socialgene-0.1.7/socialgene/utils/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:30:05.546986 socialgene-0.1.7/socialgene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 16:30:05.000000 socialgene-0.1.7/socialgene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-22 16:30:05.000000 socialgene-0.1.7/socialgene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:30:05.000000 socialgene-0.1.7/socialgene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 16:30:05.000000 socialgene-0.1.7/socialgene.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 16:30:05.000000 socialgene-0.1.7/socialgene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 16:30:05.000000 socialgene-0.1.7/socialgene.egg-info/top_level.txt
```

### Comparing `socialgene-0.1.6/LICENSE.md` & `socialgene-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/PKG-INFO` & `socialgene-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.1.6
+Version: 0.1.7
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -28,14 +28,16 @@
 # Status
 
 ## Github
 
 ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy) [![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy) [![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml) [![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml) [![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
 ## PyPI
 
+https://pypi.org/project/socialgene/
+
 ![PyPI](https://img.shields.io/pypi/v/socialgene) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socialgene) ![PyPI - Status](https://img.shields.io/pypi/status/socialgene) ![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
 
 # Contributing
 
 Please see https://github.com/socialgene/sgpy/blob/main/CONTRIBUTING.md
 
 # Documentation
```

### Comparing `socialgene-0.1.6/README.md` & `socialgene-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # Status
 
 ## Github
 
 ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy) [![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy) [![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml) [![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml) [![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
 ## PyPI
 
+https://pypi.org/project/socialgene/
+
 ![PyPI](https://img.shields.io/pypi/v/socialgene) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socialgene) ![PyPI - Status](https://img.shields.io/pypi/status/socialgene) ![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
 
 # Contributing
 
 Please see https://github.com/socialgene/sgpy/blob/main/CONTRIBUTING.md
 
 # Documentation
```

### Comparing `socialgene-0.1.6/pyproject.toml` & `socialgene-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socialgene"
-version = "0.1.6"
+version = "0.1.7"
 description = "Creating and interacting with graph databases of protein domains and their genome coordinates"
 readme = "README.md"
 authors =  [
     {name = "Chase M. Clark", email = "chasingmicrobes@gmail.com"},
 ]
 keywords = []  #! TODO
 # Pypi classifiers: https://pypi.org/classifiers/
```

### Comparing `socialgene-0.1.6/setup.cfg` & `socialgene-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/setup.py` & `socialgene-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/base/compare_protein.py` & `socialgene-0.1.7/socialgene/base/compare_protein.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/base/molbio.py` & `socialgene-0.1.7/socialgene/base/molbio.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/base/socialgene.py` & `socialgene-0.1.7/socialgene/base/socialgene.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/__main__.py` & `socialgene-0.1.7/socialgene/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/clean_hmms.py` & `socialgene-0.1.7/socialgene/cli/clean_hmms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/create_neo4j_db.py` & `socialgene-0.1.7/socialgene/cli/create_neo4j_db.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/export_neo4j_header_files.py` & `socialgene-0.1.7/socialgene/cli/export_neo4j_header_files.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/export_protein_loci_assembly_tables.py` & `socialgene-0.1.7/socialgene/cli/export_protein_loci_assembly_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/parameter_export.py` & `socialgene-0.1.7/socialgene/cli/parameter_export.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/parse_ncbi_feature_tables.py` & `socialgene-0.1.7/socialgene/cli/parse_ncbi_feature_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/parse_ncbi_taxonomy.py` & `socialgene-0.1.7/socialgene/cli/parse_ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/process_domtblout.py` & `socialgene-0.1.7/socialgene/cli/process_domtblout.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/protein_sqlite.py` & `socialgene-0.1.7/socialgene/cli/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/cli/socialgene_hmm_tsv_parser.py` & `socialgene-0.1.7/socialgene/cli/socialgene_hmm_tsv_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/clustermap/clustermap.py` & `socialgene-0.1.7/socialgene/clustermap/clustermap.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/common_parameters.env` & `socialgene-0.1.7/socialgene/common_parameters.env`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/config.py` & `socialgene-0.1.7/socialgene/config.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/data/biosample_attributes` & `socialgene-0.1.7/socialgene/data/biosample_attributes`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/findmybgc/findmybgc.py` & `socialgene-0.1.7/socialgene/findmybgc/findmybgc.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/hashing/hashing.py` & `socialgene-0.1.7/socialgene/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/hmm/hmmer.py` & `socialgene-0.1.7/socialgene/hmm/hmmer.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/hmm/hmminfo.py` & `socialgene-0.1.7/socialgene/hmm/hmminfo.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/mmseqs/create_database.py` & `socialgene-0.1.7/socialgene/mmseqs/create_database.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/mmseqs/index_database.py` & `socialgene-0.1.7/socialgene/mmseqs/index_database.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/mmseqs/search.py` & `socialgene-0.1.7/socialgene/mmseqs/search.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/admin_import.py` & `socialgene-0.1.7/socialgene/neo4j/admin_import.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/ingest_from_neo4j.py` & `socialgene-0.1.7/socialgene/neo4j/ingest_from_neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/neo4j.py` & `socialgene-0.1.7/socialgene/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/queries.cypher` & `socialgene-0.1.7/socialgene/neo4j/queries.cypher`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/schema/define_modules.py` & `socialgene-0.1.7/socialgene/neo4j/schema/define_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/schema/define_nodes.py` & `socialgene-0.1.7/socialgene/neo4j/schema/define_nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,24 +106,24 @@
         self.add_node(
             neo4j_label="mz_cluster_index",
             header_filename="mz_cluster_index_nodes.header",
             target_subdirectory="paired_omics",
             target_extension="mz_cluster_index_nodes",
             header=[
                 "uid:ID(mz_cluster_index)",
-                "component_index:Float",
-                "parent_mass:Double",
-                "precursor_mass:Double",
-                "sum_precursor_intensity:Double",
+                "component_index:Long",
+                "parent_mass:Float",
+                "precursor_mass:Float",
+                "sum_precursor_intensity:Float",
                 "Smiles:String",
-                "rt_mean::Double",
-                "rt_std_err:Double",
+                "rt_mean::Float",
+                "rt_std_err:Float",
                 "library_id:String",
-                "mq_score:Double",
-                "mz_error_ppm:Double",
+                "mq_score:Float",
+                "mz_error_ppm:Float",
                 "mass_diff:String",
             ],
         )
 
         self.add_node(
             neo4j_label="mz_source_file",
             header_filename="mz_source_file.header",
```

### Comparing `socialgene-0.1.6/socialgene/neo4j/schema/define_relationships.py` & `socialgene-0.1.7/socialgene/neo4j/schema/define_relationships.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,26 @@
             neo4j_label="ANNOTATES",
             header_filename="protein_to_hmm_header.header",
             target_subdirectory="parsed_domtblout",
             target_extension="parseddomtblout",
             header=[
                 ":END_ID(protein)",
                 ":START_ID(hmm)",
-                "env_from:Float",
-                "env_to:Float",
-                "seq_pro_score:Double",
-                "evalue:Double",
-                "i_evalue:Double",
-                "domain_bias:Double",
-                "domain_score:Double",
-                "seq_pro_bias:Double",
-                "hmm_from:Float",
-                "hmm_to:Float",
-                "ali_from:Float",
-                "ali_to:Float",
+                "env_from:Long",
+                "env_to:Long",
+                "seq_pro_score:Float",
+                "evalue:Long",
+                "i_evalue:Long",
+                "domain_bias:Float",
+                "domain_score:Float",
+                "seq_pro_bias:Float",
+                "hmm_from:Long",
+                "hmm_to:Long",
+                "ali_from:Long",
+                "ali_to:Long",
                 "exponentialized:Boolean",
             ],
         )
 
         self.add_relationship(
             neo4j_label="ASSEMBLES_TO",
             header_filename="assembly_to_locus.header",
@@ -41,22 +41,22 @@
             target_subdirectory="genomic_info",
             target_extension="locus_to_protein",
             header=[
                 ":START_ID(nucleotide)",
                 ":END_ID(protein)",
                 "protein_id",
                 "locus_tag",
-                "start:Float",
-                "end:Float",
-                "strand:Float",
+                "start:Long",
+                "end:Long",
+                "strand:Long",
                 "description",
                 "partial_on_complete_genome:Boolean",
                 "missing_start:Boolean",
                 "missing_stop:Boolean",
-                "Integerernal_stop:Boolean",
+                "internal_stop:Boolean",
                 "partial_in_the_middle_of_a_contig:Boolean",
                 "missing_N_terminus:Boolean",
                 "missing_C_terminus:Boolean",
                 "frameshifted:Boolean",
                 "too_short_partial_abutting_assembly_gap:Boolean",
                 "incomplete:Boolean",
             ],
@@ -131,25 +131,25 @@
             neo4j_label="BLASTP",
             header_filename="blastp.header",
             target_subdirectory="diamond_blastp",
             target_extension="blast6",
             header=[
                 ":START_ID(protein)",
                 ":END_ID(protein)",
-                "pident:Double",
-                "length:Float",
-                "mismatch:Float",
-                "gapopen:Float",
-                "qstart:Float",
-                "qend:Float",
-                "sstart:Float",
-                "send:Float",
-                "evalue:Double",
-                "bitscore:Double",
-                "qcovhsp:Double",
+                "pident:Float",
+                "length:Long",
+                "mismatch:Long",
+                "gapopen:Long",
+                "qstart:Long",
+                "qend:Long",
+                "sstart:Long",
+                "send:Long",
+                "evalue:Float",
+                "bitscore:Float",
+                "qcovhsp:Float",
             ],
         )
 
         self.add_relationship(
             neo4j_label="MMSEQS2",
             header_filename="mmseqs2.header",
             target_subdirectory="mmseqs2_cluster",
@@ -169,18 +169,18 @@
             neo4j_label="MOLECULAR_NETWORK",
             header_filename="molecular_network.header",
             target_subdirectory="paired_omics",
             target_extension="molecular_network",
             header=[
                 ":START_ID(mz_cluster_index)",
                 ":END_ID(mz_cluster_index)",
-                "delta_mz:double",
-                "meh:Double",
-                "cosine:Double",
-                "other_score:Double",
+                "delta_mz:Float",
+                "meh:Float",
+                "cosine:Float",
+                "other_score:Float",
             ],
         )
 
         self.add_relationship(
             neo4j_label="METABO",
             header_filename="assembly_to_mz_file.header",
             target_subdirectory="paired_omics",
```

### Comparing `socialgene-0.1.6/socialgene/neo4j/schema/node_relationship_class.py` & `socialgene-0.1.7/socialgene/neo4j/schema/node_relationship_class.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/schema/socialgene_modules.py` & `socialgene-0.1.7/socialgene/neo4j/schema/socialgene_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/search/basic.py` & `socialgene-0.1.7/socialgene/neo4j/search/basic.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/neo4j/single_protein_search.py` & `socialgene-0.1.7/socialgene/neo4j/single_protein_search.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/parsers/datasets_parse.py` & `socialgene-0.1.7/socialgene/parsers/datasets_parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/parsers/hmmer_parser.py` & `socialgene-0.1.7/socialgene/parsers/hmmer_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/parsers/hmmmodel.py` & `socialgene-0.1.7/socialgene/parsers/hmmmodel.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/parsers/ncbi_feature_table.py` & `socialgene-0.1.7/socialgene/parsers/ncbi_feature_table.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/parsers/ncbi_taxonomy.py` & `socialgene-0.1.7/socialgene/parsers/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/parsers/sequence_parser.py` & `socialgene-0.1.7/socialgene/parsers/sequence_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
             "partial_in_the_middle_of_a_contig": "partial in the middle of a contig",
             "missing_N_terminus": "missing N-terminus",
             "missing_C_terminus": "missing C-terminus",
             "frameshifted": "frameshifted",
             "too_short_partial_abutting_assembly_gap": "too short partial abutting assembly gap",
             "incomplete": "incomplete",
         }
-        return {k: True for k, v in bad_proteins.items() if re.search(v, note)}
+        # The exact string "true" is looked for by neo4j admin import, not True
+        # https://neo4j.com/docs/operations-manual/current/tools/neo4j-admin/neo4j-admin-import/#import-tool-header-format-properties
+        return {k: "true" for k, v in bad_proteins.items() if re.search(v, note)}
 
     def _process_go(self, note: str) -> Dict[str, List[str]]:
         return {"goterms": re.findall("GO:[0-9]{7}", note)}
 
     def _process_feature_note(self, seq_feature) -> Dict:
         note = {}
         if "note" in seq_feature.qualifiers:
```

### Comparing `socialgene-0.1.6/socialgene/scoring/scoring.py` & `socialgene-0.1.7/socialgene/scoring/scoring.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/chunker.py` & `socialgene-0.1.7/socialgene/utils/chunker.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/file_handling.py` & `socialgene-0.1.7/socialgene/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/get_ncbi_biosample_attributes.py` & `socialgene-0.1.7/socialgene/utils/get_ncbi_biosample_attributes.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/goterms.py` & `socialgene-0.1.7/socialgene/utils/goterms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/logging.py` & `socialgene-0.1.7/socialgene/utils/logging.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/ncbi_ftp.py` & `socialgene-0.1.7/socialgene/utils/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/nextflow_test_utils.py` & `socialgene-0.1.7/socialgene/utils/nextflow_test_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/pandas_utils.py` & `socialgene-0.1.7/socialgene/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/prep_ncbi_biosample_data.py` & `socialgene-0.1.7/socialgene/utils/prep_ncbi_biosample_data.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/protein_sqlite.py` & `socialgene-0.1.7/socialgene/utils/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/run_subprocess.py` & `socialgene-0.1.7/socialgene/utils/run_subprocess.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene/utils/untargz.py` & `socialgene-0.1.7/socialgene/utils/untargz.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene.egg-info/PKG-INFO` & `socialgene-0.1.7/socialgene.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.1.6
+Version: 0.1.7
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -28,14 +28,16 @@
 # Status
 
 ## Github
 
 ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy) [![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy) [![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml) [![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml) [![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
 ## PyPI
 
+https://pypi.org/project/socialgene/
+
 ![PyPI](https://img.shields.io/pypi/v/socialgene) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socialgene) ![PyPI - Status](https://img.shields.io/pypi/status/socialgene) ![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
 
 # Contributing
 
 Please see https://github.com/socialgene/sgpy/blob/main/CONTRIBUTING.md
 
 # Documentation
```

### Comparing `socialgene-0.1.6/socialgene.egg-info/SOURCES.txt` & `socialgene-0.1.7/socialgene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.6/socialgene.egg-info/entry_points.txt` & `socialgene-0.1.7/socialgene.egg-info/entry_points.txt`

 * *Files identical despite different names*

