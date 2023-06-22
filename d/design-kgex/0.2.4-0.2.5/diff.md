# Comparing `tmp/design_kgex-0.2.4.tar.gz` & `tmp/design_kgex-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design_kgex-0.2.4.tar", last modified: Wed Jun 21 23:29:32 2023, max compression
+gzip compressed data, was "design_kgex-0.2.5.tar", last modified: Thu Jun 22 00:11:26 2023, max compression
```

## Comparing `design_kgex-0.2.4.tar` & `design_kgex-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 23:29:32.930633 design_kgex-0.2.4/
--rw-rw-rw-   0        0        0     1134 2023-06-18 07:04:17.000000 design_kgex-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       85 2023-06-19 19:22:36.000000 design_kgex-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      295 2023-06-21 23:29:32.929637 design_kgex-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5139 2023-06-19 22:33:14.000000 design_kgex-0.2.4/README.md
--rw-rw-rw-   0        0        0       82 2023-06-19 10:38:09.000000 design_kgex-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 23:29:32.931687 design_kgex-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      624 2023-06-21 23:27:02.000000 design_kgex-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 23:29:32.815886 design_kgex-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 23:29:32.903060 design_kgex-0.2.4/src/design_kgex/
--rw-rw-rw-   0        0        0        0 2023-06-18 03:55:58.000000 design_kgex-0.2.4/src/design_kgex/__init__.py
--rw-rw-rw-   0        0        0     5900 2023-06-21 23:29:02.000000 design_kgex-0.2.4/src/design_kgex/design_knowledge.py
--rw-rw-rw-   0        0        0     6230 2023-06-21 23:27:35.000000 design_kgex-0.2.4/src/design_kgex/patent_text.py
--rw-rw-rw-   0        0        0    15722 2023-06-19 20:46:57.000000 design_kgex-0.2.4/src/design_kgex/supplementary.pkl
-drwxrwxrwx   0        0        0        0 2023-06-21 23:29:32.926387 design_kgex-0.2.4/src/design_kgex.egg-info/
--rw-rw-rw-   0        0        0      295 2023-06-21 23:29:32.000000 design_kgex-0.2.4/src/design_kgex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-06-21 23:29:32.000000 design_kgex-0.2.4/src/design_kgex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 23:29:32.000000 design_kgex-0.2.4/src/design_kgex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-21 23:29:32.000000 design_kgex-0.2.4/src/design_kgex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-21 23:29:32.000000 design_kgex-0.2.4/src/design_kgex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 00:11:26.820246 design_kgex-0.2.5/
+-rw-rw-rw-   0        0        0     1134 2023-06-18 07:04:17.000000 design_kgex-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-06-19 19:22:36.000000 design_kgex-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-06-22 00:11:26.820246 design_kgex-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5139 2023-06-19 22:33:14.000000 design_kgex-0.2.5/README.md
+-rw-rw-rw-   0        0        0       82 2023-06-19 10:38:09.000000 design_kgex-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 00:11:26.820246 design_kgex-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-06-22 00:10:40.000000 design_kgex-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:11:26.785717 design_kgex-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 00:11:26.804618 design_kgex-0.2.5/src/design_kgex/
+-rw-rw-rw-   0        0        0        0 2023-06-18 03:55:58.000000 design_kgex-0.2.5/src/design_kgex/__init__.py
+-rw-rw-rw-   0        0        0     5900 2023-06-21 23:29:02.000000 design_kgex-0.2.5/src/design_kgex/design_knowledge.py
+-rw-rw-rw-   0        0        0     6230 2023-06-21 23:27:35.000000 design_kgex-0.2.5/src/design_kgex/patent_text.py
+-rw-rw-rw-   0        0        0    15722 2023-06-19 20:46:57.000000 design_kgex-0.2.5/src/design_kgex/supplementary.pkl
+drwxrwxrwx   0        0        0        0 2023-06-22 00:11:26.820246 design_kgex-0.2.5/src/design_kgex.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-06-22 00:11:26.000000 design_kgex-0.2.5/src/design_kgex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-22 00:11:26.000000 design_kgex-0.2.5/src/design_kgex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      121 2023-06-22 00:11:26.000000 design_kgex-0.2.5/src/design_kgex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-22 00:11:26.000000 design_kgex-0.2.5/src/design_kgex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 00:11:26.000000 design_kgex-0.2.5/src/design_kgex.egg-info/top_level.txt
```

### Comparing `design_kgex-0.2.4/LICENSE` & `design_kgex-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `design_kgex-0.2.4/README.md` & `design_kgex-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `design_kgex-0.2.4/src/design_kgex/design_knowledge.py` & `design_kgex-0.2.5/src/design_kgex/design_knowledge.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.2.4/src/design_kgex/patent_text.py` & `design_kgex-0.2.5/src/design_kgex/patent_text.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.2.4/src/design_kgex/supplementary.pkl` & `design_kgex-0.2.5/src/design_kgex/supplementary.pkl`

 * *Files identical despite different names*

