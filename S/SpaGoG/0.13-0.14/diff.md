# Comparing `tmp/SpaGoG-0.13.tar.gz` & `tmp/SpaGoG-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpaGoG-0.13.tar", last modified: Tue May  9 12:40:28 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.14.tar", last modified: Thu Jun 22 20:46:02 2023, max compression
```

## Comparing `SpaGoG-0.13.tar` & `SpaGoG-0.14.tar`

### file list

```diff
@@ -1,43 +1,9 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      370 2023-05-09 12:40:28.508539 SpaGoG-0.13/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-08 23:47:17.000000 SpaGoG-0.13/README.md
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/SpaGoG.egg-info/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      370 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      915 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/SOURCES.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/dependency_links.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       29 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/requires.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/top_level.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-05-09 12:40:28.508539 SpaGoG-0.13/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      565 2023-05-09 12:40:20.000000 SpaGoG-0.13/setup.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/datasets/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7361 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphsDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphsDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/tabDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11832 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/tabDataset.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/default_params/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/default_params/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/default_params/load_params.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11778 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/experiments.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     5062 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/main.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/models/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/abstractModel.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    14164 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/abstractNN.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/graphClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    17286 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/graphNodeClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/nodeClassification.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/utils/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/utils/data/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/data/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/data/tab2graph.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/gfp.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/knn.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/utils/metrics/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/metrics/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/metrics/metrics.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:46:02.000000 SpaGoG-0.14/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1224 2023-06-22 20:38:39.000000 SpaGoG-0.14/setup.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.14/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.14/README
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      486 2023-06-22 20:46:02.000000 SpaGoG-0.14/PKG-INFO
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:46:02.000000 SpaGoG-0.14/spagog/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     8354 2023-06-22 20:21:02.000000 SpaGoG-0.14/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.14/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11750 2023-06-22 20:14:46.000000 SpaGoG-0.14/spagog/experiments.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `SpaGoG-0.13/spagog/experiments.py` & `SpaGoG-0.14/spagog/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import torch
 
-from .datasets.tabDataset import TabDataset
-from .datasets.graphsDataset import GraphsDataset
+from datasets.tabDataset import TabDataset
+from datasets.graphsDataset import GraphsDataset
 
-from .models.graphClassification import ValuesAndGraphStructure as GC
-from .models.graphNodeClassification import GraphNodeClassification as GNC
-from .models.nodeClassification import NodeClassification
+from models.graphClassification import ValuesAndGraphStructure as GC
+from models.graphNodeClassification import GraphNodeClassification as GNC
+from models.nodeClassification import NodeClassification
 
 PROJECT_DIR = "."
 
 
 def run_gc(
         tab_dataset: TabDataset,
         params: dict,
@@ -165,34 +165,36 @@
 
     cache, all_graphs_loader = model.fit(
         graphs_dataset,
         inter_samples_edges,
         train_mask,
         val_mask,
         test_mask,
-        n_epochs=10000,
+        n_epochs=600,
         gc_lr=params["gc_lr"],
         nc_lr=params["nc_lr"],
         gc_weight_decay=params["gc_weight_decay"],
         nc_weight_decay=params["nc_weight_decay"],
         alpha=params["alpha"],
         batch_size=params.get("batch_size", 10),
         early_stopping_patience=early_stopping,
         verbose=verbose,
         clf_from=params["clf_from"]  # clf_from
     )
 
-    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"], probs=False,
+    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
+                           probs=False,
                            to_numpy=to_numpy)
 
     if evaluate_metrics and verbose == 1:
         print(f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}")
 
     if probs:
-        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"], probs=True,
+        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
+                               probs=True,
                                to_numpy=to_numpy)
 
     return y_test, cache
 
 
 def run_gc_nc(
         tab_dataset: TabDataset,
@@ -342,17 +344,14 @@
 
     if probs:
         y_test = nc_model.predict(test_graph, probs=True, to_numpy=to_numpy)
 
     return y_test, cache
 
 
-def get_default_params_file(model):
-    return f"default_params/{model}.json"
-
 
 def get_tab_data(
         train_X: pd.DataFrame,
         train_Y: pd.DataFrame,
         test_X: pd.DataFrame,
         test_Y: pd.DataFrame = None,
         val_X: pd.DataFrame = None,
```

