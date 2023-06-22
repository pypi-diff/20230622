# Comparing `tmp/baguette_verse-1.0.6.3.tar.gz` & `tmp/baguette_verse-1.0.6.4.tar.gz`

## Comparing `baguette_verse-1.0.6.3.tar` & `baguette_verse-1.0.6.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/baguette.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/logger.py
--rw-r--r--   0        0        0    17676 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/rack.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/__init__.py
--rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/bake.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/compiler.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    33988 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/extractor.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/toast.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/source/evaluator.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/tutorial/data.zip
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/tutorial/scripts.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/tutorial/state.txt
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/baguette/tutorial/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/LICENSE
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/pyproject.toml
--rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/logger.py
+-rw-r--r--   0        0        0    17676 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    33988 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/LICENSE
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/PKG-INFO
```

### Comparing `baguette_verse-1.0.6.3/baguette/baguette.py` & `baguette_verse-1.0.6.4/baguette/baguette.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/logger.py` & `baguette_verse-1.0.6.4/baguette/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/rack.py` & `baguette_verse-1.0.6.4/baguette/rack.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/bake.py` & `baguette_verse-1.0.6.4/baguette/bakery/bake.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/compiler.py` & `baguette_verse-1.0.6.4/baguette/bakery/compiler.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/build.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/build.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/colors.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/colors.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/config.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/config.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/event.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/filters.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/graph.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/graph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/record.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/utils.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from .relations import InjectedThread, StartedThread
     if c.arguments.thread_identifier != 0:      # Should indicate that the call failed
         logger.debug("New thread detected.")
         t : Thread
         t, ok = find_or_create(Thread, TID = c.arguments.thread_identifier)
         l = StartedThread(c, t)
         if c.name in {"CreateRemoteThread", "CreateRemoteThreadEx"}:
-            logger.info("Detected thread injection.")
+            logger.debug("Detected thread injection.")
             l.remote = True
             p = c.thread.process
             InjectedThread(p, t)
 
 @chrono
 def integrate_process_creation(c : entities.Call):
     """
```

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/network/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/network/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             raise ValueError("'\\' not permitted in a registry key name")
         if len(value) > 255:
             raise ValueError("Key name is too long to be allowed by registry")
         self.__name = value.lower().title().replace("\x00", "\uFFFD")
         if not self.printable:
             from .....logger import logger
             from ...config import ColorSetting
-            logger.info("Got an unprintable registry key.")
+            logger.debug("Got an unprintable registry key.")
             self.color = self.unprintable_key_color
     
     @property
     def path(self) -> str:
         """
         The global key name (path from root key and all sub-keys to reach this key included).
         """
```

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/extractor.py` & `baguette_verse-1.0.6.4/baguette/croutons/extractor.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/toast.py` & `baguette_verse-1.0.6.4/baguette/croutons/toast.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.6.4/baguette/croutons/metalib/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.6.4/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.6.4/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/source/evaluator.py` & `baguette_verse-1.0.6.4/baguette/croutons/source/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.6.4/baguette/croutons/source/metagraph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/croutons/source/utils.py` & `baguette_verse-1.0.6.4/baguette/croutons/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/tutorial/data.zip` & `baguette_verse-1.0.6.4/baguette/tutorial/data.zip`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/tutorial/scripts.py` & `baguette_verse-1.0.6.4/baguette/tutorial/scripts.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/baguette/tutorial/utils.py` & `baguette_verse-1.0.6.4/baguette/tutorial/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/.gitignore` & `baguette_verse-1.0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/LICENSE` & `baguette_verse-1.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/README.md` & `baguette_verse-1.0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.3/pyproject.toml` & `baguette_verse-1.0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "1.0.6.3"
+version = "1.0.6.4"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-1.0.6.3/PKG-INFO` & `baguette_verse-1.0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.6.3
+Version: 1.0.6.4
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

