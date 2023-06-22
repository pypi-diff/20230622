# Comparing `tmp/wwpdb.apps.ccmodule-0.27.tar.gz` & `tmp/wwpdb.apps.ccmodule-0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ccmodule-0.27.tar", last modified: Tue Jun 13 11:18:38 2023, max compression
+gzip compressed data, was "wwpdb.apps.ccmodule-0.28.tar", last modified: Thu Jun 22 04:42:23 2023, max compression
```

## Comparing `wwpdb.apps.ccmodule-0.27.tar` & `wwpdb.apps.ccmodule-0.28.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/
--rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
--rw-r--r--   0 vsts      (1001) docker     (123)   121120 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)   103161 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73659 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11689 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/ccOps.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    90790 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/
--rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15516 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompReports.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6341 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/DbSession.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/
--rw-r--r--   0 vsts      (1001) docker     (123)     9350 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     7201 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28707 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/Exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7942 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/
--rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompView.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)   138698 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    96593 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2370 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 11:18:26.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.013129 wwpdb.apps.ccmodule-0.28/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   122825 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   105108 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73659 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12269 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/ccOps.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    94861 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15516 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompReports.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8576 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/DbSession.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9350 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7201 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28664 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/Exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7942 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompView.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)   138698 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    96593 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2370 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-22 04:42:07.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ccmodule-0.27/PKG-INFO` & `wwpdb.apps.ccmodule-0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.27
+Version: 0.28
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.27/setup.py` & `wwpdb.apps.ccmodule-0.28/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssign.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssign.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 # 2017-03-27    RPS    Generating cc-dpstr-info file on intermittent saves now.
 # 2017-04-11    RPS    Updates to accommodate identification of ligands selected by depositor as "ligands of interest"
 # 2017-05-03    RPS    Updates so that LOI tracking can succeed even in cases where annotator reruns ligand search and consequently changes value for "author" assigned CCID
 # 2017-05-24    RPS    Corrected for missing variable initialization in updateWithDepositorInfo().
 # 2017-09-19    ZF     Add runMultiAssignValidation() and change doAssignValidation() to multiprocessing mode
 # 2021-02-25    ZF     Add self.__origUpdIdMap & self.__sortCompositeMatchScore()
 # 2022-05-23    ZF     Move the __getDpstrOrigCcids() method call from __synchronizeDataStore() method to doAssignValidation() for multiple instances case
+# 2023-06-21    ZF     Add "pdbx_metadata_info" & "pdbx_descriptor_info" categories to chemical assign program
 ##
 """
 Residue-level chemical component extraction operations.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -95,15 +96,15 @@
 import traceback
 import inspect
 
 #
 from rcsb.utils.multiproc.MultiProcUtil import MultiProcUtil
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxChemCompAssignReader
+from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition,PdbxChemCompAssignReader
 from wwpdb.apps.ccmodule.io.ChemCompDataImport import ChemCompDataImport
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
 from wwpdb.apps.ccmodule.io.ChemCompIo import ChemCompReader
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from mmcif.io.PdbxReader import PdbxReader
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
@@ -239,14 +240,16 @@
                 (e.g. as when requested by wwPDB Common Tool Deposition UI = Lite Lig Module).
 
             :Returns:
                 ``dataDict``: return dictionary of assignment result information for
                 this deposition corresponding to cif categories:
 
                             + 'pdbx_entry_info'
+                            + 'pdbx_metadata_info'
+                            + 'pdbx_descriptor_info'
                             + 'pdbx_instance_assignment'
                             + 'pdbx_match_list'
                             + 'pdbx_atom_mapping'
                             + 'pdbx_missing_atom'
 
         """
         # the return dictionary -
@@ -368,15 +371,15 @@
 
         #########################################################################################################
         # interrogate resulting assign results file for desired match data
         #########################################################################################################
         pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
         pR.setFilePath(filePath=pathToAssignFile)
         pR.getBlock()
-        for cN in ['pdbx_entry_info', 'pdbx_instance_assignment', 'pdbx_match_list', 'pdbx_atom_mapping', 'pdbx_missing_atom']:
+        for cN in list(PdbxCategoryDefinition._cDict.keys()):
             if pR.categoryExists(cN):
                 dataDict[cN] = pR.getCategory(catName=cN)
 
         return dataDict
 
     def saveState(self, pathDict, context="annot", mode=None):
         """ Method for capturing current state of chem component assignments.
@@ -864,15 +867,15 @@
             origCcidDict = self.__getDpstrOrigCcids()
         #
         for retResult in retLists[0]:
             pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
             pR.setFilePath(filePath=retResult[1])
             pR.getBlock()
             dd = {}
-            for cN in ['pdbx_entry_info', 'pdbx_instance_assignment', 'pdbx_match_list', 'pdbx_atom_mapping', 'pdbx_missing_atom']:
+            for cN in list(PdbxCategoryDefinition._cDict.keys()):
                 if pR.categoryExists(cN):
                     dd[cN] = pR.getCategory(catName=cN)
                 #
             #
             ccADS = self.updateDataStoreForInstnc(retResult[0], dd, preFlag=flag, preCcidDict=origCcidDict)
             ccADS.serialize()
         #
@@ -987,15 +990,15 @@
             else:
                 self.__lfh.write("+ChemCompAssign.doAssignInstance() - NO assignment file created.\n")
                 ccAssignFilePath = None
 
             pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
             pR.setFilePath(filePath=ccAssignFilePath)
             pR.getBlock()
-            for cN in ['pdbx_entry_info', 'pdbx_instance_assignment', 'pdbx_match_list', 'pdbx_atom_mapping', 'pdbx_missing_atom']:
+            for cN in list(PdbxCategoryDefinition._cDict.keys()):
                 if pR.categoryExists(cN):
                     dd[cN] = pR.getCategory(catName=cN)
 
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 self.__lfh.write("+ChemCompAssign.doAssignInstance() - pre-processing failed for:  %s\n" % mdlfilePath)
                 traceback.print_exc(file=self.__lfh)
@@ -1063,15 +1066,15 @@
             else:
                 self.__lfh.write("+ChemCompAssign.doAssignInstanceComp() - NO assignment file created.\n")
                 ccAssignFilePath = None
 
             pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
             pR.setFilePath(filePath=ccAssignFilePath)
             pR.getBlock()
-            for cN in ['pdbx_entry_info', 'pdbx_instance_assignment', 'pdbx_match_list', 'pdbx_atom_mapping', 'pdbx_missing_atom']:
+            for cN in list(PdbxCategoryDefinition._cDict.keys()):
                 if pR.categoryExists(cN):
                     dd[cN] = pR.getCategory(catName=cN)
 
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 self.__lfh.write("+ChemCompAssign.doAssignInstanceComp() - pre-processing failed for:  %s\n" % mdlfilePath)
                 traceback.print_exc(file=self.__lfh)
@@ -1561,14 +1564,43 @@
                     ##
                     ###################################################
 
                 ####################################################################################################################################
                 #    END OF for-loop
                 ####################################################################################################################################
                 ####################################################################################################################################
+            #
+        #
+        if ("pdbx_metadata_info" in p_dataDict) and (len(p_dataDict["pdbx_metadata_info"]) > 0):
+            for row in p_dataDict["pdbx_metadata_info"]:
+                if ("_pdbx_metadata_info.id" not in row) or (not row["_pdbx_metadata_info.id"]):
+                    continue
+                #
+                p_ccAssgnDataStore.setAuthorProvidedRestraintFlag(row["_pdbx_metadata_info.id"])
+                #
+                for keyTupL in ( ( "name", "_pdbx_metadata_info.name" ), ( "formula", "_pdbx_metadata_info.formula" ), \
+                                 ( "natoms", "_pdbx_metadata_info.natoms" ) ):
+                    if (keyTupL[1] not in row) or (not row[keyTupL[1]]):
+                        continue
+                    #
+                    p_ccAssgnDataStore.addAuthorProvidedMetaData(row["_pdbx_metadata_info.id"], keyTupL[0], row[keyTupL[1]])
+                #
+            #
+        #
+        if ("pdbx_descriptor_info" in p_dataDict) and (len(p_dataDict["pdbx_descriptor_info"]) > 0):
+            for row in p_dataDict["pdbx_descriptor_info"]:
+                if ("_pdbx_descriptor_info.id" not in row) or (not row["_pdbx_descriptor_info.id"]) or \
+                   ("_pdbx_descriptor_info.type" not in row) or (not row["_pdbx_descriptor_info.type"]) or \
+                   ("_pdbx_descriptor_info.descriptor" not in row) or (not row["_pdbx_descriptor_info.descriptor"]):
+                    continue
+                #
+                p_ccAssgnDataStore.addAuthorProvidedDescriptor(row["_pdbx_descriptor_info.id"], row["_pdbx_descriptor_info.type"], \
+                                                               row["_pdbx_descriptor_info.descriptor"])
+            #
+        #
 
     def __ccLiteUploadFileHndling(self, p_ccADS, p_ligId=None):
         """ Method for processing any files that were uploaded by the depositor to supplement
         the data collection for the deposition. Files will be copied to workflow storage
         and file names will be registered with the ChemCompAssignDataStore for recall purposes.
         Currently, component-definition, component-image, and sdf files are recognized file types.
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 # 2014-05-22    RPS    Updates to support display of entry title in header of webpage.
 # 2014-07-09    RPS        Fix for handling outer double quotes placed on SMILES strings (during CIF persistence) when generating 2D images for depositor info.
 # 2014-11-03    ZF     Changed '.gif' to '.svg' for aligned images, added '2dpath' variable to 'cc_viz_cmp_li_tmplt.html' & 'cc_viz_cmp_li_tmplt_newcandidt.html' template
 # 2016-07-22    RPS    Added debug trace logging to track file types of files uploaded by depositor via LigandLite.
 # 2017-02-10    RPS    Implementing safeguard against crashes of OeBuildMol/OeDepict when problematic SMILES strings encountered
 # 2017-04-11    RPS    Updates to accommodate identification of ligands selected by depositor as "ligands of interest"
 # 2017-05-03    RPS    Updates so that LOI tracking can succeed even in cases where annotator reruns ligand search and consequently changes value for "author" assigned CCID
+# 2023-06-21    ZF     Added chemical descriptions provided by refinement packages
 ##
 """
 Create HTML depiction chemical component assignment files.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -150,14 +151,15 @@
                                    'dpstr_info_sketch_sdf_img_pth',
                                    'dpstr_info_sketch_sdf_img_lnk',
                                    'dpstr_info_image',
                                    'dpstr_info_image_lnk',
                                    'dpstr_info_dscrptr',
                                    'dpstr_info_dscrptr_type',
                                    'dpstr_info_dscrptr_img_pth',
+                                   'dpstr_restraint_img_pth',
                                    'dpstr_info_type',
                                    'dpstr_info_details']
 
     ################################################################################################################
     # ------------------------------------------------------------------------------------------------------------
     #      Top-level methods
     # ------------------------------------------------------------------------------------------------------------
@@ -551,14 +553,21 @@
             displayClass = ''
             buttonLbl = "Hide Rerun Search Form"
         else:
             displayClass = 'displaynone'
             buttonLbl = "Show Rerun Search Form"
         lclDict['rerun_display_class'] = displayClass
         lclDict['rerun_btn_lbl'] = buttonLbl
+        #
+        author_info_display_class = 'displaynone'
+        if p_ccAssgnDataStr.hasAuthorProvidedRestraintFlag(p_authAssignedGrp) and \
+           os.access(os.path.join(self.absltAssgnSessionPath, p_authAssignedGrp, p_authAssignedGrp + ".cif"), os.F_OK):
+            author_info_display_class = ''
+        #
+        lclDict['author_info_display_class'] = author_info_display_class
         ##
         ############################################################
         #
         dsplyvizopt = "displaynone"
         for instId in p_instncIdLst:
 
             grp = p_ccAssgnDataStr.getAuthAssignment(instId)
@@ -583,15 +592,15 @@
         # ## dpstr info handling ###
         lclDict['display_dpstr_info'] = "displaynone"
         lclDict['display_dscrptr_vw_btn'] = "displaynone"
         naStr = "n/a"
         #
         for keyName in self.__dpstrInfoKeyList:
             lclDict[keyName] = naStr
-        if p_authAssignedGrp in p_ccAssgnDataStr.getGlbllyRslvdGrpList():
+        if (p_authAssignedGrp in p_ccAssgnDataStr.getGlbllyRslvdGrpList()) or p_ccAssgnDataStr.hasAuthorProvidedRestraintFlag(p_authAssignedGrp):
             self.__packDpstrViewDict(p_authAssignedGrp, p_ccAssgnDataStr, lclDict)
         for keyName in self.__dpstrInfoKeyList:
             lclDict[keyName + "_displ"] = "displaynone" if lclDict[keyName] == naStr else ""
         ###########################
         lclDict['all_instncs_profile_view'] = self.processTemplate(tmpltPth=htmlTmpltPth, fn="cc_all_instncs_profile_tmplt.html", parameterDict=lclDict)
         p_oL.append(self.processTemplate(tmpltPth=htmlTmpltPth, fn="cc_all_instncs_disp_tmplt.html", parameterDict=lclDict))
         # ############################# END creating "all instances" view ##############################
@@ -1326,15 +1335,15 @@
         lclDict['display_dpstr_info'] = "displaynone"
         lclDict['display_dscrptr_vw_btn'] = "displaynone"
         naStr = "n/a"
         #
         for keyName in self.__dpstrInfoKeyList:
             lclDict[keyName] = naStr
         ccAssgnDataStr = ChemCompAssignDataStore(p_reqObj, verbose=True, log=self.__lfh)
-        if authAssngdGrp in ccAssgnDataStr.getGlbllyRslvdGrpList():
+        if (authAssngdGrp in ccAssgnDataStr.getGlbllyRslvdGrpList()) or ccAssgnDataStr.hasAuthorProvidedRestraintFlag(authAssngdGrp):
             self.__packDpstrViewDict(authAssngdGrp, ccAssgnDataStr, lclDict)
         for keyName in self.__dpstrInfoKeyList:
             lclDict[keyName + "_displ"] = "displaynone" if lclDict[keyName] == naStr else ""
         ###########################
 
         oL.append(self.processTemplate(tmpltPth=os.path.join(tmpltPath, self.__pathAllInstcs), fn="cc_dpstr_info_vw_tmplt.html", parameterDict=lclDict))
 
@@ -1356,25 +1365,44 @@
         # ## dpstr info handling ###
         naStr = "n/a"
         contentTypeDict = self.__cI.get('CONTENT_TYPE_DICTIONARY')
 
         ligType = p_dataStore.getDpstrCcType(p_grpId)
         altLigId = p_dataStore.getDpstrAltCcId(p_grpId)
         chemCompName = p_dataStore.getDpstrCcName(p_grpId)
+        if (chemCompName is None) or (chemCompName == "?"):
+            name = p_dataStore.getAuthorProvidedMetaData(p_grpId, "name")
+            if name:
+                chemCompName = name
+            #
+        #
         chemCompFrmla = p_dataStore.getDpstrCcFrmla(p_grpId)
+        if (chemCompFrmla is None) or (chemCompFrmla == "?"):
+            formula = p_dataStore.getAuthorProvidedMetaData(p_grpId, "formula")
+            if formula:
+                chemCompFrmla = formula
+            #
+        #
         chemCompDescriptor = p_dataStore.getDpstrCcDscrptrStr(p_grpId)
         chemCompDescriptorType = p_dataStore.getDpstrCcDscrptrType(p_grpId)
+        if (chemCompDescriptor is None) or (chemCompDescriptor == "?") or (chemCompDescriptorType is None) or (chemCompDescriptorType == "?"):
+            desType,desStr = p_dataStore.getAuthorProvidedDescriptorInfo(p_grpId)
+            if desType and desStr:
+                chemCompDescriptor = desStr
+                chemCompDescriptorType = desType
+            #
+        #
         chemCompDetails = p_dataStore.getDpstrComments(p_grpId)
         p_strReplDict['display_dpstr_info'] = ""
-        p_strReplDict['dpstr_info_name'] = chemCompName if chemCompName != '?' else naStr
-        p_strReplDict['dpstr_info_alt_comp_id'] = altLigId if altLigId != '?' else naStr
-        p_strReplDict['dpstr_info_frmla'] = chemCompFrmla if chemCompFrmla != '?' else naStr
+        p_strReplDict['dpstr_info_name'] = chemCompName if chemCompName and (chemCompName != '?') else naStr
+        p_strReplDict['dpstr_info_alt_comp_id'] = altLigId if altLigId and (altLigId != '?') else naStr
+        p_strReplDict['dpstr_info_frmla'] = chemCompFrmla if chemCompFrmla and (chemCompFrmla != '?') else naStr
 
-        p_strReplDict['dpstr_info_dscrptr'] = chemCompDescriptor if chemCompDescriptor != '?' else naStr
-        p_strReplDict['dpstr_info_dscrptr_type'] = chemCompDescriptorType if chemCompDescriptorType != '?' else naStr
+        p_strReplDict['dpstr_info_dscrptr'] = chemCompDescriptor if chemCompDescriptor and (chemCompDescriptor != '?') else naStr
+        p_strReplDict['dpstr_info_dscrptr_type'] = chemCompDescriptorType if chemCompDescriptorType and (chemCompDescriptorType != '?') else naStr
 
         if chemCompDescriptorType and chemCompDescriptorType.lower() == 'smiles':
 
             try:
                 # creating 2D image representation of the SMILES string
                 fileName = p_grpId + "_dscrptr_depict.svg"
                 toLclSessnImgPth = os.path.join(self.absltAssgnSessionPath, fileName)
@@ -1416,16 +1444,16 @@
                 #
         else:
             p_strReplDict['display_dscrptr_vw_btn'] = "displaynone"
             p_strReplDict['dpstr_info_dscrptr_img_pth'] = ""
             if self.__verbose:
                 self.__lfh.write("+%s.%s() - no SMILES string submitted for this ligand ID [%s].\n" % (className, methodName, p_grpId))
 
-        p_strReplDict['dpstr_info_type'] = ligType if ligType != '?' else naStr
-        p_strReplDict['dpstr_info_details'] = chemCompDetails if chemCompDetails != '?' else naStr
+        p_strReplDict['dpstr_info_type'] = ligType if ligType and (ligType != '?') else naStr
+        p_strReplDict['dpstr_info_details'] = chemCompDetails if chemCompDetails and (chemCompDetails != '?') else naStr
 
         for contentType in contentTypeDict['component-image'][0]:
             imageFileList = p_dataStore.getDpstrUploadFile(p_grpId, contentType)
             if self.__verbose and self.__debug:
                 self.__lfh.write("\n++++ChemCompAssignDepict.__packDpstrViewDict() ----- contentTypeDict['component-image'][0] %r\n" % contentTypeDict['component-image'][0])
                 self.__lfh.write("\n++++ChemCompAssignDepict.__packDpstrViewDict() ----- imageFileList %r\n" % imageFileList)
 
@@ -1450,14 +1478,19 @@
         sketchFileList = p_dataStore.getDpstrSketchFile(p_grpId)
         self.__lfh.write("\n++++ChemCompAssignDepict.__packDpstrViewDict() ----- sketchFileList %r\n" % sketchFileList)
         if sketchFileList is not None:
             fileName = sketchFileList[0]
             p_strReplDict['dpstr_info_sketch_sdf'] = fileName
             p_strReplDict['dpstr_info_sketch_sdf_lnk'] = '<a href="' + os.path.join(self.rltvAssgnSessionPath, fileName) + '" target="_blank">' + fileName + '</a>'
             p_strReplDict['dpstr_info_sketch_sdf_img_pth'] = os.path.join(self.rltvAssgnSessionPath, p_grpId + ".svg")
+        #
+        restraintImagePath = os.path.join(self.absltAssgnSessionPath, p_grpId, "image", p_grpId + ".svg")
+        if os.access(restraintImagePath, os.F_OK):
+            p_strReplDict['dpstr_restraint_img_pth'] = os.path.join(self.rltvAssgnSessionPath, p_grpId, "image", p_grpId + ".svg")
+        #
 
     def __renderInstance3dViews(self, p_ccAssgnDataStr, p_hlprDict):
         ''' For given ligand instance id, generates html fragments used for 3D jmol viewing in the "single-instance view"
             and "all-instances view" comparison panels-->these are written to files on server to be used on demand
 
             :Params:
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # 2011-06-14    RPS    Updated for addition of following items as per update to data models:
 #                            _pdbx_instance_assignment.warning_message
 #                            _pdbx_instance_assignment.parameter
 #                            and
 #                            _pdbx_match_list.warning_message
 # 2011-06-20    RPS    Updated for update to _pdbx_match_list category definition
 # 2012-10-24    RPS    Updated to reflect reorganization of modules in pdbx packages
+# 2023-06-21    ZF     Added 'pdbx_metadata_info' & 'pdbx_descriptor_info' catetories
 ##
 """
 A collection of classes supporting chemical component assignment data files.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -44,14 +45,23 @@
             ('_pdbx_entry_info.format', '%s', 'str', ''),
             ('_pdbx_entry_info.number_of_total', '%s', 'str', ''),
             ('_pdbx_entry_info.number_of_passed', '%s', 'str', ''),
             ('_pdbx_entry_info.number_of_match', '%s', 'str', ''),
             ('_pdbx_entry_info.number_of_close_match', '%s', 'str', ''),
             ('_pdbx_entry_info.number_of_no_match', '%s', 'str', ''),
             ('_pdbx_entry_info.status', '%s', 'str', '')],
+        'pdbx_metadata_info': [
+            ('_pdbx_metadata_info.id', '%s', 'str', ''),
+            ('_pdbx_metadata_info.name', '%s', 'str', ''),
+            ('_pdbx_metadata_info.formula', '%s', 'str', ''),
+            ('_pdbx_metadata_info.natoms', '%s', 'str', '')],
+        'pdbx_descriptor_info': [
+            ('_pdbx_descriptor_info.id', '%s', 'str', ''),
+            ('_pdbx_descriptor_info.type', '%s', 'str', ''),
+            ('_pdbx_descriptor_info.descriptor', '%s', 'str', '')],
         'pdbx_instance_assignment': [
             ('_pdbx_instance_assignment.inst_id', '%s', 'str', ''),
             ('_pdbx_instance_assignment.het_id', '%s', 'str', ''),
             ('_pdbx_instance_assignment.single_atom_flag', '%s', 'str', ''),
             ('_pdbx_instance_assignment.status', '%s', 'str', ''),
             ('_pdbx_instance_assignment.warning_message', '%s', 'str', ''),
             ('_pdbx_instance_assignment.parameter', '%s', 'str', '')
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/ChemCompDepict.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/ChemCompDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/ccOps.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/ccOps.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 # 2017-02-12    RPS    Removing canned text for capture of "details" data for ligands as "focus of research"
 # 2017-02-13    RPS    Updates to distinguish between ligandIDs that were simply selected as focus of research vs those for which data was actually provided.
 # 2017-02-14    RPS    generateUpdatedDepInfoFile updated --> correcting "auth_sym_id" to "auth_asym_id"
 # 2017-02-15    RPS    generateUpdatedDepInfoFile updated --> output complete pdbx_entity_instance_feature category
 # 2017-02-17    RPS    generateUpdatedDepInfoFile updated --> accommodating new "auth_comp_id" item for "pdbx_binding_assay category"
 # 2017-03-30    RPS    now generating cc-dpstr-prgrss file when there are no ligands requiring attention (in support of depui monitoring at module launch)
 # 2017-05-03    RPS    Updates so that LOI tracking can succeed even in cases where annotator reruns ligand search and consequently changes value for "author" assigned CCID
+# 2023-06-21    ZF     Added self.__authorProvidedInfo dict to hold chemical description information provided by refinement packages
 ##
 '''
 Provide a storage interface for recording chemical component
 assignment data/state for given deposition data set when
 being processed via the common tool ligand module
 
 '''
@@ -172,14 +173,17 @@
         #                                 # so that authoritative precedence given to most recent uploads
         self.__rsrchAcqurdGrpLst = []     # admin/convenience list for keeping track of entity groups for which data was captured for "focus of research" needs.
         self.__dpstrCcRsrchInfo = {}  # dictionary mapping ligand code to research data provied by depositor
         self.__rsrchSlctdGrpLst = []     # admin/convenience list for keeping track of entity groups which were indicated as "focus of research".
         self.__dpstrOrigCcIdMaster = {}  # Authoritative copy of CCID which depositor had originally used to identify the ligand
         # ###################Chem Comp Lite attributes END   ###############################
 
+        self.__authorProvidedInfo = {} # Metadata and chemical descriptor(s) information provided by depositor from extra data block(s) 
+                                       # where new chemical information are stored.
+
         self.__setup()
 
     def __setup(self):
         """ Setup of a given ChemCompAssignDataStore object involves checking for an existing
             serialized pickle file for the current deposition dataset being processed.
             If such a pickle file exists, we use it to populate the object with the last recorded
             state of chemical component search results and annotator assignments.
@@ -310,14 +314,15 @@
         self.__rslvdPrtnCntr = 1
         self.__rslvdPrtnDict = {}
         self.__dpstrUpldFlsOrder = {}
         self.__rsrchAcqurdGrpLst = []
         self.__dpstrCcRsrchInfo = {}
         self.__rsrchSlctdGrpLst = []
         self.__dpstrOrigCcIdMaster = {}
+        self.__authorProvidedInfo = {}
 
     def serialize(self):
         """ Persist data to a pickle file on server so that state can be maintained
             between web requests within a given ligand module session
         """
         if self.__verbose:
             self.__lfh.write("+ChemCompAssignStore.serialize() - starting\n")
@@ -365,14 +370,15 @@
             pickle.dump(self.__rslvdPrtnCntr, fb, self.__pickleProtocol)
             pickle.dump(self.__rslvdPrtnDict, fb, self.__pickleProtocol)
             pickle.dump(self.__dpstrUpldFlsOrder, fb, self.__pickleProtocol)
             pickle.dump(self.__rsrchAcqurdGrpLst, fb, self.__pickleProtocol)
             pickle.dump(self.__dpstrCcRsrchInfo, fb, self.__pickleProtocol)
             pickle.dump(self.__rsrchSlctdGrpLst, fb, self.__pickleProtocol)
             pickle.dump(self.__dpstrOrigCcIdMaster, fb, self.__pickleProtocol)
+            pickle.dump(self.__authorProvidedInfo, fb, self.__pickleProtocol)
             fb.close()
         except:  # noqa: E722 pylint: disable=bare-except
             self.__lfh.write("+ChemCompAssignStore.serialize() - exception encountered\n")
             traceback.print_exc(file=self.__lfh)
 
     def deserialize(self):
         """ Pull data from a pickle file on server into memory so that state can be
@@ -422,14 +428,15 @@
             self.__rslvdPrtnCntr = pickle.load(fb)
             self.__rslvdPrtnDict = pickle.load(fb)
             self.__dpstrUpldFlsOrder = pickle.load(fb)
             self.__rsrchAcqurdGrpLst = pickle.load(fb)
             self.__dpstrCcRsrchInfo = pickle.load(fb)
             self.__rsrchSlctdGrpLst = pickle.load(fb)
             self.__dpstrOrigCcIdMaster = pickle.load(fb)
+            self.__authorProvidedInfo = pickle.load(fb)
 
             fb.close()
 
             # below for loops are defensive measure for backwards compatibility of older pickle files
             # that may have been created prior to introduction of the given dictionary attributes
             for ligId in self.__GlbllyRslvdGrpLst:
                 if not (ligId in self.__rslvdPrtnDict):
@@ -1404,14 +1411,108 @@
         try:
             return self.__dpstrOrigCcIdMaster[instId]
         except:  # noqa: E722 pylint: disable=bare-except
             return None
 
     #########################################################################
 
+    def setAuthorProvidedRestraintFlag(self, grpId):
+        try:
+            if grpId not in self.__authorProvidedInfo:
+                self.__authorProvidedInfo[grpId] = {}
+            #
+            self.__authorProvidedInfo[grpId]["restraint"] = "YES"
+            return True
+        except:  # noqa: E722 pylint: disable=bare-except
+            return False
+        #
+
+    def hasAuthorProvidedRestraintFlag(self, grpId):
+        try:
+            if (grpId in self.__authorProvidedInfo) and ("restraint" in self.__authorProvidedInfo[grpId]):
+               if self.__authorProvidedInfo[grpId]["restraint"] == "YES":
+                   return True
+                #
+            #
+            return False
+        except:  # noqa: E722 pylint: disable=bare-except
+            return False
+        #
+
+    def getAuthorProvidedRestraintGrpIds(self):
+        try:
+            grpIdList = []
+            for grpId,valD in self.__authorProvidedInfo.items():
+                if ("restraint" in valD) and (valD["restraint"] == "YES"):
+                    grpIdList.append(grpId)
+                #
+            #
+            return grpIdList
+        except:  # noqa: E722 pylint: disable=bare-except
+            return []
+        #
+
+    def addAuthorProvidedMetaData(self, grpId, key, val):
+        try:
+            if grpId not in self.__authorProvidedInfo:
+                self.__authorProvidedInfo[grpId] = {}
+            #
+            self.__authorProvidedInfo[grpId][key] = val
+            return True
+        except:  # noqa: E722 pylint: disable=bare-except
+            return False
+        #
+
+    def getAuthorProvidedMetaData(self, grpId, key):
+        try:
+            if (grpId in self.__authorProvidedInfo) and (key in self.__authorProvidedInfo[grpId]):
+                return self.__authorProvidedInfo[grpId][key]
+            #
+            return None
+        except:  # noqa: E722 pylint: disable=bare-except
+            return None
+        #
+
+    def addAuthorProvidedDescriptor(self, grpId, descriptorType, descriptorVal):
+        try:
+            if grpId not in self.__authorProvidedInfo:
+                self.__authorProvidedInfo[grpId] = {}
+            #
+            if "descriptor" not in self.__authorProvidedInfo[grpId]:
+                self.__authorProvidedInfo[grpId]["descriptor"] = {}
+            #
+            self.__authorProvidedInfo[grpId]["descriptor"][descriptorType] = descriptorVal
+            return True
+        except:  # noqa: E722 pylint: disable=bare-except
+            return False
+        #
+
+    def getAuthorProvidedDescriptor(self, grpId, descriptorType):
+        try: 
+            if (grpId in self.__authorProvidedInfo) and ("descriptor" in self.__authorProvidedInfo[grpId]) and \
+               (descriptorType in self.__authorProvidedInfo[grpId]["descriptor"]):
+                return self.__authorProvidedInfo[grpId]["descriptor"][descriptorType]
+            #
+            return None
+        except:  # noqa: E722 pylint: disable=bare-except
+            return None
+        #
+
+    def getAuthorProvidedDescriptorInfo(self, grpId):
+        try: 
+            if (grpId in self.__authorProvidedInfo) and ("descriptor" in self.__authorProvidedInfo[grpId]) and \
+               (len(self.__authorProvidedInfo[grpId]["descriptor"]) > 0):
+                itemList = sorted(self.__authorProvidedInfo[grpId]["descriptor"].items())
+                return itemList[-1]
+            #
+            return None,None
+        except:  # noqa: E722 pylint: disable=bare-except
+            return None,None
+        #
+
     def setDpstrAltCcId(self, grpId, altId):
         try:
             if altId is None:
                 del self.__dpstrCcAltId[grpId]
             else:
                 self.__dpstrCcAltId[grpId] = altId
         except:  # noqa: E722 pylint: disable=bare-except
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataExport.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataImport.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompEditStore.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompEditStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompIo.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompReports.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompReports.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompView.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,177 +1,172 @@
 ##
-# File:  InstanceDataGenerator.py
-# Date:  27-feb-2015
+# File:  ChemCompView.py
+# Date:  29-Jul-2010
+# Updates:
+# ---------------------------------------------------------------------------
+# 2011-05-12  RPS  Piloting changes to doView() and getChemCompInfo() for standalone Ligand Editor Tool
+# 2011-08-05  RPS  Updated with comments in support of generating "restructuredtext" documentation
+# 2011-08-17  RPS  Updated so that ChemCompViewDepict uses inherited setSessionPaths() function from ChemCompDepict
+#                     for establishing absolute and relative paths used for session data management
+# 2012-10-24  RPS  Updated to reflect reorganization of modules in pdbx packages
 ##
 """
-Utility Class for generating report material that will support 2D,3D renderings.
-
-This software was developed as part of the World Wide Protein Data Bank
-Common Deposition and Annotation System Project
-
-Copyright (c) 2012 wwPDB
-
-This software is provided under a Creative Commons Attribution 3.0 Unported
-License described at http://creativecommons.org/licenses/by/3.0/.
+Create simple web views from chemical component definitions.
 
 """
 __docformat__ = "restructuredtext en"
-__author__ = "Zukang Feng"
-__email__ = "zfeng@rcsb.rutgers.edu"
+__author__ = "John Westbrook"
+__email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.01"
 
 import os
 import sys
-import multiprocessing
-import traceback
 
-from wwpdb.apps.ccmodule.reports.ChemCompAlignImageGenerator import ChemCompAlignImageGenerator
 from wwpdb.apps.ccmodule.reports.ChemCompReports import ChemCompReport
-#
+from wwpdb.apps.ccmodule.view.ChemCompViewDepict import ChemCompViewDepict
+from mmcif_utils.chemcomp.PdbxChemCompIo import PdbxChemCompIo
 
 
-class InstanceDataGenerator(object):
-    """Utility Class for generating report material that will support 2D,3D renderings.
+class ChemCompView(object):
+    """Create simple web views from chemical component definitions.
+
     """
-    def __init__(self, reqObj=None, dataStore=None, verbose=False, log=sys.stderr):
-        self.__reqObj = reqObj
-        self.__ccAssignDataStore = dataStore
+    def __init__(self, reqObj, verbose=False, log=sys.stderr):
+        """Create simple web views from chemical component definitions.
+
+         :param `verbose`:  boolean flag to activate verbose logging.
+         :param `log`:      stream for logging.
+
+        """
         self.__verbose = verbose
         self.__lfh = log
+        self.__debug = True
         #
-        # Leave the following call due to potential side effects.
-        self.__sObj = self.__reqObj.getSessionObj()  # pylint: disable=unused-private-member
-        # self.__sessionPath = self.__sObj.getPath()
+        self.__reqObj = reqObj
+        #
+        # self.__sobj=self.__reqObj.newSessionObj()
         #
+        # self.__sObj = self.__reqObj.getSessionObj()
+        # self.__sessionPath = self.__sObj.getPath()
+        # self.__sessionRelativePath = self.__sObj.getRelativePath()
 
-    def run(self):
-        # depId = str(self.__reqObj.getValue("identifier")).upper()
-        instIdLst = self.__ccAssignDataStore.getAuthAssignmentKeys()
-        if len(instIdLst) == 0:
-            return
-        #
-        refList = []
-        for instId in instIdLst:
-            mtchL = self.__ccAssignDataStore.getTopHitsList(instId)
-            for tupL in mtchL:
-                refList.append(tupL[0])
-            #
-        #
-        if len(refList) > 0:
-            uniqList = sorted(set(refList))
-            rrG = RefReportGenerator(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-            self.__runMultiprocessing(uniqList, rrG, 'runReportGenerator')
         #
-        irG = InstReportGenerator(reqObj=self.__reqObj, dataStore=self.__ccAssignDataStore, verbose=self.__verbose, log=self.__lfh)
-        self.__runMultiprocessing(instIdLst, irG, 'runReportGenerator')
+        self.__idList = []  # pylint: disable=unused-private-member
+        #
 
-    def __runMultiprocessing(self, dataList, workerObj, workerMethod):
-        """
+    def setIdList(self, idList):
+        self.__idList = idList  # pylint: disable=unused-private-member
+
+    def doView(self):
+        """ Call to display data for given chem component in comparison grid of standalone version of chem comp module.
+
+            :Helpers:
+
+                + wwpdb.apps.ccmodule.reports.ChemCompReports.ChemCompReport
+                + wwpdb.apps.ccmodule.view.ChemCompViewDepict.ChemCompViewDepict
+
+            :Returns:
+                ``rtrnCode``: integer indicating success of this operation
+                    -1: failure
+                    0: success
         """
-        numProc = int(multiprocessing.cpu_count() / 2)
-        if numProc == 0:
-            numProc = 1
-        #
-        if numProc > len(dataList):
-            numProc = len(dataList)
-        #
-        subLists = [dataList[i::numProc] for i in range(numProc)]
-        workerFunc = getattr(workerObj, workerMethod)
-        #
-        taskQueue = multiprocessing.Queue()
-        resultQueue = multiprocessing.Queue()
-        #
-        workers = [MultiProcWorker(processLabel=str(i + 1), taskQueue=taskQueue, resultQueue=resultQueue,
-                                   workerFunc=workerFunc, log=self.__lfh, verbose=self.__verbose) for i in range(numProc)]
-        for w in workers:
-            w.start()
-        #
-        for subList in subLists:
-            taskQueue.put(subList)
-        #
-        for i in range(numProc):
-            taskQueue.put(None)
-        #
-        for i in range(len(subLists)):
-            _msg = resultQueue.get()  # noqa: F841
-        #
-        try:
-            for w in workers:
-                w.terminate()
-                w.join(1)
-            #
-        except:  # noqa: E722 pylint: disable=bare-except
+        # determine which chem component is to be viewed (i.e. which chem comp ID has been passed in request)
+        ccId = str(self.__reqObj.getValue("ccid")).upper()
+        # return code indicating failure by default
+        rtrnCode = -1
+        #############################################################################################################
+        #        Generate report material for requested dictionary reference
+        #############################################################################################################
+        ccReferncRprt = ChemCompReport(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
+        ccReferncRprt.setDefinitionId(definitionId=ccId)
+        ccReferncRprt.doReport()
+        rD = ccReferncRprt.getReportFilePaths()
+        for k, v in rD.items():
             if self.__verbose:
-                traceback.print_exc(file=self.__lfh)
-            #
-        #
-
+                self.__lfh.write("+ChemCompView._doView() -- Reference file reporting -- Key %30s value %s\n" % (k, v))
+        ##########################################################
+        # interrogate report data in order to get name and
+        # formula for the chem component reference
+        #########################################################
+        # ccRefFilePath=os.path.join(self.__sessionPath,ccId,'report',ccId+'.cif')
+        ccRefFilePath = ccReferncRprt.getFilePath()
+        #
+        if os.access(ccRefFilePath, os.R_OK):
+            chemCompD = self.getChemCompInfo(ccRefFilePath, ccId)
+            rtrnCode = 0
+            if self.__verbose:
+                self.__lfh.write("+ChemCompView._doView() - successfully processing chem comp ID %s with name %s and formula %s\n" %
+                                 (chemCompD['id'], chemCompD['name'], chemCompD['formula']))
 
-class MultiProcWorker(multiprocessing.Process):
-    """
-    """
-    def __init__(self, processLabel='', taskQueue=None, resultQueue=None, workerFunc=None, log=sys.stderr, verbose=False):  # pylint: disable=unused-argument
-        multiprocessing.Process.__init__(self)
-        self.__processLabel = processLabel
-        self.__taskQueue = taskQueue
-        self.__resultQueue = resultQueue
-        self.__workerFunc = workerFunc
-        # self.__lfh = log
-        # self.__verbose = verbose
-
-    def run(self):
-        while True:
-            nextList = self.__taskQueue.get()
-            if nextList is None:
-                break
-            #
-            self.__workerFunc(dataList=nextList, processLabel=self.__processLabel)
-            self.__resultQueue.put("OK")
+        else:
+            if self.__verbose:
+                self.__lfh.write("+ChemCompView._doView() - NO reference chem comp file found for %s\n" % ccRefFilePath)
+        #
+        #########################################################
+        # call render() methods to generate html markup to be supplied for display in comparison grid
+        ccVD = ChemCompViewDepict(self.__verbose, self.__lfh)
+        ccVD.setSessionPaths(self.__reqObj)
+        # ccVD.doRender_ccRefForViewer(chemCompTupl,self.__reqObj)
+        ccVD.doRender(chemCompD, self.__reqObj)
         #
 
+        return rtrnCode
 
-class RefReportGenerator(object):
-    """
-    """
-    def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
-        self.__reqObj = reqObj
-        self.__verbose = verbose
-        self.__lfh = log
-        #
+    def getChemCompInfo(self, cifPath, ccId):
+        """ Extract data to be displayed for given chem component from cif definition file
 
-    def runReportGenerator(self, dataList=None, processLabel=None):  # pylint: disable=unused-argument
-        ccReport = ChemCompReport(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-        for ccId in dataList:
-            ccReport.setDefinitionId(definitionId=ccId.lower())
-            ccReport.doReport(type='ref', ccAssignPthMdfier=ccId)
-        #
+            :Params:
 
+                + ``cifPath``: path to cif chem component definition file for the given ccId
+                + ``ccId`` : ID for chemical component for which info is being requested
 
-class InstReportGenerator(object):
-    """
-    """
-    def __init__(self, reqObj=None, dataStore=None, verbose=False, log=sys.stderr):
-        self.__ccAssignDataStore = dataStore
-        self.__reqObj = reqObj
-        self.__verbose = verbose
-        self.__lfh = log
-        #
-        self.__sObj = self.__reqObj.getSessionObj()
-        self.__sessionPath = self.__sObj.getPath()
-        #
+            :Helpers:
+                mmcif_utils.chemcomp.PdbxChemCompIo.PdbxChemCompIo
 
-    def runReportGenerator(self, dataList=None, processLabel=None):  # pylint: disable=unused-argument
-        for instId in dataList:
-            chemCompFilePathAbs = os.path.join(self.__sessionPath, 'assign', instId, instId + '.cif')
-            instChemCompRprt = ChemCompReport(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-            instChemCompRprt.setFilePath(chemCompFilePathAbs, instId)
-            instChemCompRprt.doReport(type='exp', ccAssignPthMdfier=instId)
-            #
-            mtchL = self.__ccAssignDataStore.getTopHitsList(instId)
-            HitList = []
-            for tupL in mtchL:
-                HitList.append(tupL[0])
-            #
-            ccaig = ChemCompAlignImageGenerator(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-            ccaig.generateImages(instId=instId, instFile=chemCompFilePathAbs, hitList=HitList)
-        #
+            :Returns:
+                ``ccDict``: dictionary of chem comp fields to be displayed for the given ccId
+        """
+        ccDict = {}
+        if os.path.exists(cifPath):
+            ccf = PdbxChemCompIo(verbose=self.__verbose, log=self.__lfh)
+            ccf.setFilePath(cifPath, compId=ccId)
+            ccf.getComp()
+            ccDL = ccf.getChemCompDict()
+            if (len(ccDL) < 1):
+                return ccDict
+
+            ccD = ccDL[0]
+            if (self.__verbose):
+                for k, v in ccD.items():
+                    self.__lfh.write("+ChemCompView.getChemCompInfo() key %20s  value %s\n" % (k, v))
+
+            ccDict['id'] = ccD['_chem_comp.id']
+            ccDict['status'] = ccD['_chem_comp.pdbx_release_status']
+            ccDict['replaced'] = ccD['_chem_comp.pdbx_replaced_by']
+            ccDict['replaces'] = ccD['_chem_comp.pdbx_replaces']
+            ccDict['name'] = ccD['_chem_comp.name']
+            ccDict['formula'] = ccD['_chem_comp.formula']
+            ccDict['formal_charge'] = ccD['_chem_comp.pdbx_formal_charge']
+            ccDict['synonyms'] = ccD['_chem_comp.pdbx_synonyms']
+            ccDict['subcomplist'] = ccD['_chem_comp.pdbx_subcomponent_list']
+            ccDict['creator'] = ccD['_chem_comp.pdbx_processing_site']
+            ccDict['mod_date'] = ccD['_chem_comp.pdbx_modified_date']
+            ccDict['nstd_parent'] = ccD['_chem_comp.mon_nstd_parent_comp_id']
+            ccDict['type'] = ccD['_chem_comp.type']
+            ccDict['pdbx_type'] = ccD['_chem_comp.pdbx_type']
+
+        if (self.__debug):
+            for k, v in ccDict.items():
+                self.__lfh.write("+ChemCompView.getChemCompInfo() key %20s  value %s\n" % (k, v))
+
+        return ccDict
+
+    # def __addWordBreakAtHyphen(self, iString):
+    #     oString = ""
+    #     for i in iString:
+    #         if i == '-':
+    #             oString += i
+    #             oString += "<wbr />"
+    #         else:
+    #             oString += i
+    #     return oString
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearch.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/DbSession.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/DbSession.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompConfig.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompConfig.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import shutil
 from logging import getLogger, StreamHandler, Formatter, DEBUG, INFO
 from wwpdb.apps.ccmodule.chem.ChemCompAssign import ChemCompAssign
 from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
 from wwpdb.apps.ccmodule.utils.LigandAnalysisState import LigandAnalysisState
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
-from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxChemCompAssignReader
+from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition,PdbxChemCompAssignReader
 from wwpdb.apps.ccmodule.chem.ChemCompAssignDepictLite import ChemCompAssignDepictLite
 from wwpdb.utils.session.WebRequest import InputRequest
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
@@ -182,15 +182,15 @@
         if self._verbose:
             self._logger.debug('Reading assign results for desired match data.')
 
         pR = PdbxChemCompAssignReader(self._verbose, self._lfh)
         pR.setFilePath(filePath=fPath)
         pR.getBlock()
 
-        for cN in ['pdbx_entry_info', 'pdbx_instance_assignment', 'pdbx_match_list', 'pdbx_atom_mapping', 'pdbx_missing_atom']:
+        for cN in list(PdbxCategoryDefinition._cDict.keys()):
             if pR.categoryExists(cN):
                 dataDict[cN] = pR.getCategory(catName=cN)
 
         return dataDict
 
     def _genLigandReportData(self, instId, instanceCcAbsFilePath=None, rtype='ref'):
         """Generate the actual report file. The file path is based on
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/Exceptions.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/wsgi.py` & `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/PKG-INFO` & `wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.27
+Version: 0.28
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/SOURCES.txt` & `wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

