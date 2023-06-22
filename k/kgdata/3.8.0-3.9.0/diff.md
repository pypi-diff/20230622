# Comparing `tmp/kgdata-3.8.0.tar.gz` & `tmp/kgdata-3.9.0.tar.gz`

## Comparing `kgdata-3.8.0.tar` & `kgdata-3.9.0.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 kgdata-3.8.0/Cargo.toml
--rw-r--r--   0     1001      123     1064 2023-06-15 05:46:14.000000 kgdata-3.8.0/LICENSE
--rw-r--r--   0     1001      123      747 2023-06-15 05:46:14.000000 kgdata-3.8.0/README.md
--rw-r--r--   0     1001      123     1551 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/bench/entity_design.rs
--rw-r--r--   0     1001      123      441 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/bench/mod.rs
--rw-r--r--   0     1001      123    33142 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/conversions.rs
--rw-r--r--   0     1001      123     6414 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/db.rs
--rw-r--r--   0     1001      123      743 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/error.rs
--rw-r--r--   0     1001      123      581 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/lib.rs
--rw-r--r--   0     1001      123      527 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/class.rs
--rw-r--r--   0     1001      123     2254 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/entity.rs
--rw-r--r--   0     1001      123      245 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/entity_link.rs
--rw-r--r--   0     1001      123      426 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/entity_metadata.rs
--rw-r--r--   0     1001      123      545 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/mod.rs
--rw-r--r--   0     1001      123      648 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/multilingual.rs
--rw-r--r--   0     1001      123     3399 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/property.rs
--rw-r--r--   0     1001      123     5137 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/models/value.rs
--rw-r--r--   0     1001      123    14046 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/pyo3helper/macros.rs
--rw-r--r--   0     1001      123      924 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/pyo3helper/mod.rs
--rw-r--r--   0     1001      123       16 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/mod.rs
--rw-r--r--   0     1001      123     3114 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/models/entity.rs
--rw-r--r--   0     1001      123     1133 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/models/entity_metadata.rs
--rw-r--r--   0     1001      123    10911 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/models/iterators.rs
--rw-r--r--   0     1001      123     1201 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/models/mod.rs
--rw-r--r--   0     1001      123     2187 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/models/multilingual.rs
--rw-r--r--   0     1001      123     8070 2023-06-15 05:46:14.000000 kgdata-3.8.0/src/python/models/value.rs
--rw-r--r--   0     1001      123     1498 2023-06-15 05:46:14.000000 kgdata-3.8.0/pyproject.toml
--rw-r--r--   0     1001      123    43877 2023-06-15 05:46:14.000000 kgdata-3.8.0/Cargo.lock
--rw-r--r--   0     1001      123     6129 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dataset.py
--rw-r--r--   0     1001      123       43 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/misc/__init__.py
--rw-r--r--   0     1001      123     6267 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/misc/ntriples_parser.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/__init__.py
--rw-r--r--   0     1001      123     1401 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdentitymetadata.py
--rw-r--r--   0     1001      123     7559 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdvalue.py
--rw-r--r--   0     1001      123     1138 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/__init__.py
--rw-r--r--   0     1001      123     1577 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdstatement.py
--rw-r--r--   0     1001      123     5859 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdproperty.py
--rw-r--r--   0     1001      123     3739 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdclass.py
--rw-r--r--   0     1001      123     1829 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/multilingual.py
--rw-r--r--   0     1001      123      639 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdentitylabel.py
--rw-r--r--   0     1001      123      428 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdentitylink.py
--rw-r--r--   0     1001      123     8252 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/wdentity.py
--rw-r--r--   0     1001      123     1259 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/models/propertystats.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/__init__.py
--rw-r--r--   0     1001      123     2435 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_metadata.py
--rw-r--r--   0     1001      123     9153 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_pagerank.py
--rw-r--r--   0     1001      123     2426 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/property_domains.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/__init__.py
--rw-r--r--   0     1001      123     1819 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/class_count.py
--rw-r--r--   0     1001      123     5067 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/classes.py
--rw-r--r--   0     1001      123     1604 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_types.py
--rw-r--r--   0     1001      123     2893 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_ids.py
--rw-r--r--   0     1001      123     1447 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_redirection_dump.py
--rw-r--r--   0     1001      123     6010 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_redirections.py
--rw-r--r--   0     1001      123     1345 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_dump.py
--rw-r--r--   0     1001      123     1908 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/__main__.py
--rw-r--r--   0     1001      123     1873 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/property_count.py
--rw-r--r--   0     1001      123     3104 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/page_ids.py
--rw-r--r--   0     1001      123     1294 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/page_dump.py
--rw-r--r--   0     1001      123     2454 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entity_wikilinks.py
--rw-r--r--   0     1001      123     8986 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/entities.py
--rw-r--r--   0     1001      123     1201 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/wp2wd.py
--rw-r--r--   0     1001      123     4682 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/properties.py
--rw-r--r--   0     1001      123     2965 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/datasets/property_ranges.py
--rw-r--r--   0     1001      123     1786 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/wikidata_prefixes.yml
--rw-r--r--   0     1001      123    16555 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/__main__.py
--rw-r--r--   0     1001      123     2674 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/config.py
--rw-r--r--   0     1001      123     6623 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/extra_ent_db.py
--rw-r--r--   0     1001      123    18452 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikidata/db.py
--rw-r--r--   0     1001      123       42 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/prelude.py
--rw-r--r--   0     1001      123       27 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/models/__init__.py
--rw-r--r--   0     1001      123     3721 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/models/linked_html_table.py
--rw-r--r--   0     1001      123     3470 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/models/html_article.py
--rw-r--r--   0     1001      123     1356 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/models/page_article.py
--rw-r--r--   0     1001      123     5053 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/wikiapi.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/__init__.py
--rw-r--r--   0     1001      123     8221 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/easy_tables.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/__init__.py
--rw-r--r--   0     1001      123     4166 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/grouped_articles.py
--rw-r--r--   0     1001      123     2910 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/articles.py
--rw-r--r--   0     1001      123     1754 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/__main__.py
--rw-r--r--   0     1001      123     1454 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/relational_tables.py
--rw-r--r--   0     1001      123     1983 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/easy_tables_metadata.py
--rw-r--r--   0     1001      123     1584 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/html_articles.py
--rw-r--r--   0     1001      123     2600 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/html_tables.py
--rw-r--r--   0     1001      123     4428 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/datasets/linked_relational_tables.py
--rw-r--r--   0     1001      123     2805 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/misc.py
--rw-r--r--   0     1001      123     2040 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/wikipedia/config.py
--rw-r--r--   0     1001      123     6777 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/splitter.py
--rw-r--r--   0     1001      123    13686 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/spark.py
--rw-r--r--   0     1001      123    13843 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/instances_extraction.py
--rw-r--r--   0     1001      123      138 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/prelude.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/__init__.py
--rw-r--r--   0     1001      123      648 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/infobox_property_dump.py
--rw-r--r--   0     1001      123        0 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/__init__.py
--rw-r--r--   0     1001      123     3914 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/wikilinks.py
--rw-r--r--   0     1001      123     1426 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/__main__.py
--rw-r--r--   0     1001      123     2040 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/page_ids.py
--rw-r--r--   0     1001      123      603 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/page_id_dump.py
--rw-r--r--   0     1001      123      608 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/datasets/wikilink_dump.py
--rw-r--r--   0     1001      123    12214 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/dbpediamodels.py
--rw-r--r--   0     1001      123    37449 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/table_extraction.py
--rw-r--r--   0     1001      123      417 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/table_tests.py
--rw-r--r--   0     1001      123     1886 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/dbpedia/config.py
--rw-r--r--   0     1001      123      364 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/config.py
--rw-r--r--   0     1001      123     1100 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/core/base.pyi
--rw-r--r--   0     1001      123       27 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/core/__init__.pyi
--rw-r--r--   0     1001      123     5507 2023-06-15 05:46:14.000000 kgdata-3.8.0/kgdata/core/models.pyi
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 kgdata-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 kgdata-3.9.0/Cargo.toml
+-rw-r--r--   0     1001      123     1064 2023-06-22 01:45:33.000000 kgdata-3.9.0/LICENSE
+-rw-r--r--   0     1001      123      747 2023-06-22 01:45:33.000000 kgdata-3.9.0/README.md
+-rw-r--r--   0     1001      123     1551 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/bench/entity_design.rs
+-rw-r--r--   0     1001      123      441 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/bench/mod.rs
+-rw-r--r--   0     1001      123    33142 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/conversions.rs
+-rw-r--r--   0     1001      123     6414 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/db.rs
+-rw-r--r--   0     1001      123      743 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/error.rs
+-rw-r--r--   0     1001      123      581 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/lib.rs
+-rw-r--r--   0     1001      123      527 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/class.rs
+-rw-r--r--   0     1001      123     2254 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/entity.rs
+-rw-r--r--   0     1001      123      245 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/entity_link.rs
+-rw-r--r--   0     1001      123      426 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/entity_metadata.rs
+-rw-r--r--   0     1001      123      545 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/mod.rs
+-rw-r--r--   0     1001      123      648 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/multilingual.rs
+-rw-r--r--   0     1001      123     3399 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/property.rs
+-rw-r--r--   0     1001      123     5137 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/models/value.rs
+-rw-r--r--   0     1001      123    16249 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/pyo3helper/macros.rs
+-rw-r--r--   0     1001      123     1069 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/pyo3helper/mod.rs
+-rw-r--r--   0     1001      123       16 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/mod.rs
+-rw-r--r--   0     1001      123     3114 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/entity.rs
+-rw-r--r--   0     1001      123     1133 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/entity_metadata.rs
+-rw-r--r--   0     1001      123    10911 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/iterators.rs
+-rw-r--r--   0     1001      123     1304 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/mod.rs
+-rw-r--r--   0     1001      123     2187 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/multilingual.rs
+-rw-r--r--   0     1001      123     1064 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/property.rs
+-rw-r--r--   0     1001      123     8070 2023-06-22 01:45:33.000000 kgdata-3.9.0/src/python/models/value.rs
+-rw-r--r--   0     1001      123     1498 2023-06-22 01:45:33.000000 kgdata-3.9.0/pyproject.toml
+-rw-r--r--   0     1001      123    43877 2023-06-22 01:45:33.000000 kgdata-3.9.0/Cargo.lock
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/__init__.py
+-rw-r--r--   0     1001      123       42 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/prelude.py
+-rw-r--r--   0     1001      123     2805 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/misc.py
+-rw-r--r--   0     1001      123       27 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/models/__init__.py
+-rw-r--r--   0     1001      123     1356 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/models/page_article.py
+-rw-r--r--   0     1001      123     3721 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/models/linked_html_table.py
+-rw-r--r--   0     1001      123     3470 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/models/html_article.py
+-rw-r--r--   0     1001      123     5053 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/wikiapi.py
+-rw-r--r--   0     1001      123     2040 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/config.py
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/__init__.py
+-rw-r--r--   0     1001      123     1584 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/html_articles.py
+-rw-r--r--   0     1001      123     1454 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/relational_tables.py
+-rw-r--r--   0     1001      123     8221 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/easy_tables.py
+-rw-r--r--   0     1001      123     4428 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/linked_relational_tables.py
+-rw-r--r--   0     1001      123     1983 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/easy_tables_metadata.py
+-rw-r--r--   0     1001      123     2600 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/html_tables.py
+-rw-r--r--   0     1001      123     1754 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/__main__.py
+-rw-r--r--   0     1001      123     4166 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/grouped_articles.py
+-rw-r--r--   0     1001      123     2910 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikipedia/datasets/articles.py
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/__init__.py
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/__init__.py
+-rw-r--r--   0     1001      123      138 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/prelude.py
+-rw-r--r--   0     1001      123    37449 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/table_extraction.py
+-rw-r--r--   0     1001      123    13843 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/instances_extraction.py
+-rw-r--r--   0     1001      123    12214 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/dbpediamodels.py
+-rw-r--r--   0     1001      123      417 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/table_tests.py
+-rw-r--r--   0     1001      123     1886 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/config.py
+-rw-r--r--   0     1001      123     2040 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/page_ids.py
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/__init__.py
+-rw-r--r--   0     1001      123      603 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/page_id_dump.py
+-rw-r--r--   0     1001      123     3914 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/wikilinks.py
+-rw-r--r--   0     1001      123      648 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/infobox_property_dump.py
+-rw-r--r--   0     1001      123      608 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/wikilink_dump.py
+-rw-r--r--   0     1001      123     1426 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dbpedia/datasets/__main__.py
+-rw-r--r--   0     1001      123     6006 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/core/models.pyi
+-rw-r--r--   0     1001      123     1385 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/core/base.pyi
+-rw-r--r--   0     1001      123       27 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/core/__init__.pyi
+-rw-r--r--   0     1001      123       43 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/misc/__init__.py
+-rw-r--r--   0     1001      123     6267 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/misc/ntriples_parser.py
+-rw-r--r--   0     1001      123     6129 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/dataset.py
+-rw-r--r--   0     1001      123     6777 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/splitter.py
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/__init__.py
+-rw-r--r--   0     1001      123     1786 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/wikidata_prefixes.yml
+-rw-r--r--   0     1001      123    18452 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/db.py
+-rw-r--r--   0     1001      123     6623 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/extra_ent_db.py
+-rw-r--r--   0     1001      123     1138 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/__init__.py
+-rw-r--r--   0     1001      123     1401 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdentitymetadata.py
+-rw-r--r--   0     1001      123     1259 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/propertystats.py
+-rw-r--r--   0     1001      123     3739 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdclass.py
+-rw-r--r--   0     1001      123      428 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdentitylink.py
+-rw-r--r--   0     1001      123     7559 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdvalue.py
+-rw-r--r--   0     1001      123     1829 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/multilingual.py
+-rw-r--r--   0     1001      123     5859 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdproperty.py
+-rw-r--r--   0     1001      123      639 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdentitylabel.py
+-rw-r--r--   0     1001      123     1577 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdstatement.py
+-rw-r--r--   0     1001      123     8252 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/models/wdentity.py
+-rw-r--r--   0     1001      123     2674 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/config.py
+-rw-r--r--   0     1001      123    16555 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/__main__.py
+-rw-r--r--   0     1001      123     3104 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/page_ids.py
+-rw-r--r--   0     1001      123        0 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/__init__.py
+-rw-r--r--   0     1001      123     9153 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_pagerank.py
+-rw-r--r--   0     1001      123     8986 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entities.py
+-rw-r--r--   0     1001      123     2893 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_ids.py
+-rw-r--r--   0     1001      123     1294 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/page_dump.py
+-rw-r--r--   0     1001      123     6010 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_redirections.py
+-rw-r--r--   0     1001      123     1819 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/class_count.py
+-rw-r--r--   0     1001      123     1345 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_dump.py
+-rw-r--r--   0     1001      123     2454 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_wikilinks.py
+-rw-r--r--   0     1001      123     4682 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/properties.py
+-rw-r--r--   0     1001      123     1604 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_types.py
+-rw-r--r--   0     1001      123     1873 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/property_count.py
+-rw-r--r--   0     1001      123     1447 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_redirection_dump.py
+-rw-r--r--   0     1001      123     1908 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/__main__.py
+-rw-r--r--   0     1001      123     2965 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/property_ranges.py
+-rw-r--r--   0     1001      123     5067 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/classes.py
+-rw-r--r--   0     1001      123     2426 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/property_domains.py
+-rw-r--r--   0     1001      123     2435 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/entity_metadata.py
+-rw-r--r--   0     1001      123     1201 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/wikidata/datasets/wp2wd.py
+-rw-r--r--   0     1001      123    13686 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/spark.py
+-rw-r--r--   0     1001      123      364 2023-06-22 01:45:33.000000 kgdata-3.9.0/kgdata/config.py
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 kgdata-3.9.0/PKG-INFO
```

### Comparing `kgdata-3.8.0/Cargo.toml` & `kgdata-3.9.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "kgdata"
-version = "3.0.0"
+version = "3.1.0"
 edition = "2021"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/kgdata"
 repository = "https://github.com/binh-vu/kgdata"
 license-file = "LICENSE"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 keywords = ["knowledge-graph", "wikidata", "wikipedia", "dbpedia"]
```

### Comparing `kgdata-3.8.0/LICENSE` & `kgdata-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/README.md` & `kgdata-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/bench/entity_design.rs` & `kgdata-3.9.0/src/bench/entity_design.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/conversions.rs` & `kgdata-3.9.0/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/db.rs` & `kgdata-3.9.0/src/db.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/error.rs` & `kgdata-3.9.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/lib.rs` & `kgdata-3.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/models/class.rs` & `kgdata-3.9.0/src/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/models/entity.rs` & `kgdata-3.9.0/src/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/models/mod.rs` & `kgdata-3.9.0/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/models/multilingual.rs` & `kgdata-3.9.0/src/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/models/property.rs` & `kgdata-3.9.0/src/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/models/value.rs` & `kgdata-3.9.0/src/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/pyo3helper/macros.rs` & `kgdata-3.9.0/src/pyo3helper/macros.rs`

 * *Files 12% similar despite different names*

```diff
@@ -110,14 +110,79 @@
 ///
 /// # Placeholder
 ///
 /// * structname: name of the module that will contains the mapview
 /// * module: name of the python module that will contains this struct
 /// * name: name of the python class in the module
 /// * derivetrait: optional, list of traits to derive for the struct
+/// * itemview: the item view type (a pyo3 class) -- expect to have a constructor `new(&item)`
+/// * item: the item type (rust struct)
+///
+/// # Example
+///
+/// # TODO: add example
+#[macro_export]
+macro_rules! pyset {
+    ($structname:ident (module = $module:literal, name = $name:literal, item = $item:ty as $itemview:ty $(, derive = ($( $derivetrait:ident ),*) )? )) => {
+        pub mod $structname {
+            use kgdata::pyo3helper::unsafe_update_view_lifetime_signature;
+            use pyo3::prelude::*;
+
+            #[pyclass(module = $module, name = $name)]
+            pub struct SetView(pub &'static hashbrown::HashSet<$item>);
+            #[pyclass]
+            pub struct IterView(pub hashbrown::hash_set::Iter<'static, $item>);
+
+            impl SetView {
+                pub fn new(lst: &hashbrown::HashSet<$item>) -> Self {
+                    Self(unsafe_update_view_lifetime_signature(lst))
+                }
+            }
+
+            #[pymethods]
+            impl SetView {
+                fn __iter__(&self) -> IterView {
+                    IterView(self.0.iter())
+                }
+
+                fn __len__(&self) -> usize {
+                    self.0.len()
+                }
+
+                fn __contains__(&self, item: $itemview) -> bool {
+                    self.0.contains(item.0)
+                }
+            }
+
+            #[pymethods]
+            impl IterView {
+                pub fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
+                    slf
+                }
+
+                pub fn __next__(&mut self) -> Option<$itemview> {
+                    if let Some(v) = self.0.next() {
+                        Some(<$itemview>::new(v))
+                    } else {
+                        None
+                    }
+                }
+            }
+        }
+    };
+}
+
+/// Generating a temporary map view of a Rust's map. This view allows random access at O(1) cost.
+///
+/// # Placeholder
+///
+/// * structname: name of the module that will contains the mapview
+/// * module: name of the python module that will contains this struct
+/// * name: name of the python class in the module
+/// * derivetrait: optional, list of traits to derive for the struct
 /// * key: the key type (rust struct)
 /// * keyview: the key view type -- assume that we can get the key by calling `keyview.0` and it has a constructor `new(&key)`
 /// * value: the value type (rust struct)
 /// * valueview: the value view type (a pyo3 class) -- expect to have a constructor `new(&value)`
 ///
 /// # Example
 ///
```

### Comparing `kgdata-3.8.0/src/python/models/entity.rs` & `kgdata-3.9.0/src/python/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/python/models/entity_metadata.rs` & `kgdata-3.9.0/src/python/models/entity_metadata.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/python/models/iterators.rs` & `kgdata-3.9.0/src/python/models/iterators.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/python/models/mod.rs` & `kgdata-3.9.0/src/python/models/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 use pyo3::prelude::*;
 
 pub mod entity;
 pub mod entity_metadata;
 pub mod multilingual;
+pub mod property;
 pub mod value;
 
 pub use self::entity::*;
 pub use self::entity_metadata::*;
 pub use self::multilingual::*;
+pub use self::property::*;
 pub use self::value::*;
 
 #[allow(dead_code)]
 pub(crate) fn register(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     let submodule = PyModule::new(py, "models")?;
 
     m.add_submodule(submodule)?;
 
     submodule.add_class::<self::entity::EntityView>()?;
     submodule.add_class::<self::entity::PyEntity>()?;
     submodule.add_class::<self::entity::StatementView>()?;
     submodule.add_class::<self::entity::SiteLinkView>()?;
     submodule.add_class::<self::entity_metadata::PyEntityMetadata>()?;
+    submodule.add_class::<self::property::PyProperty>()?;
     submodule.add_class::<self::value::ValueView>()?;
     submodule.add_class::<self::value::PyValue>()?;
     submodule.add_class::<self::value::PyEntityId>()?;
     submodule.add_class::<self::value::PyTime>()?;
     submodule.add_class::<self::value::PyQuantity>()?;
     submodule.add_class::<self::value::PyGlobeCoordinate>()?;
     submodule.add_class::<self::value::PyMonolingualText>()?;
```

### Comparing `kgdata-3.8.0/src/python/models/multilingual.rs` & `kgdata-3.9.0/src/python/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/src/python/models/value.rs` & `kgdata-3.9.0/src/python/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/pyproject.toml` & `kgdata-3.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kgdata"
-version = "3.8.0"
+version = "3.9.0"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 readme = "README.md"
 authors = [
     { name = "Binh Vu", email = "binh@toan2.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `kgdata-3.8.0/Cargo.lock` & `kgdata-3.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -796,15 +796,15 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kgdata"
-version = "3.0.0"
+version = "3.1.0"
 dependencies = [
  "anyhow",
  "bincode",
  "bzip2",
  "criterion",
  "env_logger",
  "flate2",
```

### Comparing `kgdata-3.8.0/kgdata/dataset.py` & `kgdata-3.9.0/kgdata/dataset.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/misc/ntriples_parser.py` & `kgdata-3.9.0/kgdata/misc/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdentitymetadata.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdentitymetadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdvalue.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdvalue.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/__init__.py` & `kgdata-3.9.0/kgdata/wikidata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdstatement.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdstatement.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdproperty.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdproperty.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdclass.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdclass.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/multilingual.py` & `kgdata-3.9.0/kgdata/wikidata/models/multilingual.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdentitylabel.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdentitylabel.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/wdentity.py` & `kgdata-3.9.0/kgdata/wikidata/models/wdentity.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/models/propertystats.py` & `kgdata-3.9.0/kgdata/wikidata/models/propertystats.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_metadata.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_pagerank.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_pagerank.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/property_domains.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/property_domains.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/class_count.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/classes.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_types.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_ids.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_redirection_dump.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_redirections.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_dump.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/__main__.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/property_count.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/property_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/page_ids.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/page_dump.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/page_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entity_wikilinks.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entity_wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/entities.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/wp2wd.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/wp2wd.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/properties.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/datasets/property_ranges.py` & `kgdata-3.9.0/kgdata/wikidata/datasets/property_ranges.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/wikidata_prefixes.yml` & `kgdata-3.9.0/kgdata/wikidata/wikidata_prefixes.yml`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/__main__.py` & `kgdata-3.9.0/kgdata/wikidata/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/config.py` & `kgdata-3.9.0/kgdata/wikidata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/extra_ent_db.py` & `kgdata-3.9.0/kgdata/wikidata/extra_ent_db.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikidata/db.py` & `kgdata-3.9.0/kgdata/wikidata/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/models/linked_html_table.py` & `kgdata-3.9.0/kgdata/wikipedia/models/linked_html_table.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/models/html_article.py` & `kgdata-3.9.0/kgdata/wikipedia/models/html_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/models/page_article.py` & `kgdata-3.9.0/kgdata/wikipedia/models/page_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/wikiapi.py` & `kgdata-3.9.0/kgdata/wikipedia/wikiapi.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/easy_tables.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/easy_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/grouped_articles.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/grouped_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/articles.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/__main__.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/relational_tables.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/easy_tables_metadata.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/easy_tables_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/html_articles.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/html_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/html_tables.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/html_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/datasets/linked_relational_tables.py` & `kgdata-3.9.0/kgdata/wikipedia/datasets/linked_relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/misc.py` & `kgdata-3.9.0/kgdata/wikipedia/misc.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/wikipedia/config.py` & `kgdata-3.9.0/kgdata/wikipedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/splitter.py` & `kgdata-3.9.0/kgdata/splitter.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/spark.py` & `kgdata-3.9.0/kgdata/spark.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/instances_extraction.py` & `kgdata-3.9.0/kgdata/dbpedia/instances_extraction.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/datasets/infobox_property_dump.py` & `kgdata-3.9.0/kgdata/dbpedia/datasets/infobox_property_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/datasets/wikilinks.py` & `kgdata-3.9.0/kgdata/dbpedia/datasets/wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/datasets/__main__.py` & `kgdata-3.9.0/kgdata/dbpedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/datasets/page_ids.py` & `kgdata-3.9.0/kgdata/dbpedia/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/datasets/page_id_dump.py` & `kgdata-3.9.0/kgdata/dbpedia/datasets/page_id_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/datasets/wikilink_dump.py` & `kgdata-3.9.0/kgdata/dbpedia/datasets/wikilink_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/dbpediamodels.py` & `kgdata-3.9.0/kgdata/dbpedia/dbpediamodels.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/table_extraction.py` & `kgdata-3.9.0/kgdata/dbpedia/table_extraction.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/dbpedia/config.py` & `kgdata-3.9.0/kgdata/dbpedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.8.0/kgdata/core/base.pyi` & `kgdata-3.9.0/kgdata/core/base.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,23 @@
     def __len__(self) -> int: ...
     def __getitem__(self, index: int) -> V: ...
 
 class RustVecIterView(Generic[V]):
     def __iter__(self) -> RustVecIterView[V]: ...
     def __next__(self) -> V: ...
 
+class RustSetView(Generic[V]):
+    def __iter__(self) -> RustSetIterView[V]: ...
+    def __len__(self) -> int: ...
+    def __contains__(self, value: V) -> bool: ...
+
+class RustSetIterView(Generic[V]):
+    def __iter__(self) -> RustSetIterView[V]: ...
+    def __next__(self) -> V: ...
+
 class RustMapView(Generic[K, V]):
     def keys(self) -> RustMapKeysView[K, V]: ...
     def values(self) -> RustMapValuesView[K, V]: ...
     def items(self) -> RustMapItemsView[K, V]: ...
     def __iter__(self) -> RustMapKeysView[K, V]: ...
     def __len__(self) -> int: ...
     def __getitem__(self, key: K) -> V: ...
```

### Comparing `kgdata-3.8.0/kgdata/core/models.pyi` & `kgdata-3.9.0/kgdata/core/models.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     KeysView,
     Literal,
     Optional,
     TypeVar,
     ValuesView,
 )
 
-from kgdata.core.base import RustMapView, RustVecView
+from kgdata.core.base import RustMapView, RustVecView, RustSetView
 
 V = TypeVar("V")
 
 EntityType = Literal["item", "property"]
 
 class EntityView:
     id: str
@@ -43,14 +43,30 @@
     aliases: MultiLingualStringListView
     instanceof: RustVecView[str]
     subclassof: RustVecView[str]
     subpropertyof: RustVecView[str]
 
     def get_all_aliases(self) -> list[str]: ...
 
+class Property:
+    id: str
+    label: MultiLingualStringView
+    description: MultiLingualStringView
+    aliases: MultiLingualStringListView
+    parents: RustVecView[str]
+    related_properties: RustVecView[str]
+    equivalent_properties: RustVecView[str]
+    subjects: RustVecView[str]
+    inverse_properties: RustVecView[str]
+    instanceof: RustVecView[str]
+    ancestors: RustSetView[str]
+
+    def is_object_property(self) -> bool: ...
+    def is_data_property(self) -> bool: ...
+
 class SiteLinkView:
     site: str
     title: str
     badges: RustVecView[str]
     url: Optional[str]
 
 class StatementView:
```

### Comparing `kgdata-3.8.0/PKG-INFO` & `kgdata-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgdata
-Version: 3.8.0
+Version: 3.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: orjson >=3.9.0, <4.0.0
 Requires-Dist: tqdm >=4.64.0, <5.0.0
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: pyspark >=3.3.0, <4.0.0
 Requires-Dist: loguru >=0.6.0, <0.7.0
```

