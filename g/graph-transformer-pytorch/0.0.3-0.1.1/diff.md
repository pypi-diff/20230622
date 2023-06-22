# Comparing `tmp/graph-transformer-pytorch-0.0.3.tar.gz` & `tmp/graph-transformer-pytorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-transformer-pytorch-0.0.3.tar", last modified: Thu Jan 13 04:32:28 2022, max compression
+gzip compressed data, was "graph-transformer-pytorch-0.1.1.tar", last modified: Thu Jun 22 14:42:09 2023, max compression
```

## Comparing `graph-transformer-pytorch-0.0.3.tar` & `graph-transformer-pytorch-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 04:32:28.072025 graph-transformer-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-13 04:32:17.000000 graph-transformer-pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-01-13 04:32:28.072025 graph-transformer-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2022-01-13 04:32:17.000000 graph-transformer-pytorch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 04:32:28.068025 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-13 04:32:17.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4526 2022-01-13 04:32:17.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch/graph_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 04:32:28.072025 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-01-13 04:32:28.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-01-13 04:32:28.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 04:32:28.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-13 04:32:28.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-13 04:32:28.000000 graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-13 04:32:28.072025 graph-transformer-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-01-13 04:32:17.000000 graph-transformer-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:42:09.346110 graph-transformer-pytorch-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 14:41:59.000000 graph-transformer-pytorch-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-22 14:42:09.346110 graph-transformer-pytorch-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-22 14:41:59.000000 graph-transformer-pytorch-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:42:09.346110 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 14:41:59.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-22 14:41:59.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch/graph_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:42:09.346110 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-22 14:42:09.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-22 14:42:09.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:42:09.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 14:42:09.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 14:42:09.000000 graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:42:09.346110 graph-transformer-pytorch-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-22 14:41:59.000000 graph-transformer-pytorch-0.1.1/setup.py
```

### Comparing `graph-transformer-pytorch-0.0.3/LICENSE` & `graph-transformer-pytorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graph-transformer-pytorch-0.0.3/PKG-INFO` & `graph-transformer-pytorch-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: graph-transformer-pytorch
-Version: 0.0.3
+Version: 0.1.1
 Summary: Graph Transformer - Pytorch
 Home-page: https://github.com/lucidrains/graph-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,graphs
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `graph-transformer-pytorch-0.0.3/README.md` & `graph-transformer-pytorch-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -30,14 +30,39 @@
 mask = torch.ones(1, 128).bool()
 
 nodes, edges = model(nodes, edges, mask = mask)
 
 nodes.shape # (1, 128, 256) - project to R^3 for coordinates
 ```
 
+If you want it to handle an adjacency matrix
+
+```python
+import torch
+from graph_transformer_pytorch import GraphTransformer
+
+model = GraphTransformer(
+    dim = 256,
+    depth = 6,
+    edge_dim = 512,
+    with_feedforwards = True,
+    gated_residual = True,
+    rel_pos_emb = True,
+    accept_adjacency_matrix = True  # set this to True
+)
+
+nodes = torch.randn(2, 128, 256)
+adj_mat = torch.randint(0, 2, (2, 128, 128))
+mask = torch.ones(2, 128).bool()
+
+nodes, edges = model(nodes, adj_mat = adj_mat, mask = mask)
+
+nodes.shape # (1, 128, 256) - project to R^3 for coordinates
+```
+
 ## Citations
 
 ```bibtex
 @article {Costa2021.06.02.446809,
     author  = {Costa, Allan and Ponnapati, Manvitha and Jacobson, Joseph M. and Chatterjee, Pranam},
     title   = {Distillation of MSA Embeddings to Folded Protein Structures with Graph Transformers},
     year    = {2021},
```

#### html2text {}

```diff
@@ -8,33 +8,41 @@
 assumed to be the same as the node dimensions above with_feedforwards = True, #
 whether to add a feedforward after each attention layer, suggested by
 literature to be needed gated_residual = True, # to use the gated residual to
 prevent over-smoothing rel_pos_emb = True # set to True if the nodes are
 ordered, default to False ) nodes = torch.randn(1, 128, 256) edges =
 torch.randn(1, 128, 128, 512) mask = torch.ones(1, 128).bool() nodes, edges =
 model(nodes, edges, mask = mask) nodes.shape # (1, 128, 256) - project to R^3
-for coordinates ``` ## Citations ```bibtex @article {Costa2021.06.02.446809,
-author = {Costa, Allan and Ponnapati, Manvitha and Jacobson, Joseph M. and
-Chatterjee, Pranam}, title = {Distillation of MSA Embeddings to Folded Protein
-Structures with Graph Transformers}, year = {2021}, doi = {10.1101/
-2021.06.02.446809}, publisher = {Cold Spring Harbor Laboratory}, URL = {https:/
-/www.biorxiv.org/content/early/2021/06/02/2021.06.02.446809}, eprint = {https:/
-/www.biorxiv.org/content/early/2021/06/02/2021.06.02.446809.full.pdf}, journal
-= {bioRxiv} } ``` ```bibtex @article {Baek2021.06.14.448402, author = {Baek,
-Minkyung and DiMaio, Frank and Anishchenko, Ivan and Dauparas, Justas and
-Ovchinnikov, Sergey and Lee, Gyu Rie and Wang, Jue and Cong, Qian and Kinch,
-Lisa N. and Schaeffer, R. Dustin and Mill{\'a}n, Claudia and Park, Hahnbeom and
-Adams, Carson and Glassman, Caleb R. and DeGiovanni, Andy and Pereira, Jose H.
-and Rodrigues, Andria V. and van Dijk, Alberdina A. and Ebrecht, Ana C. and
-Opperman, Diederik J. and Sagmeister, Theo and Buhlheller, Christoph and
-Pavkov-Keller, Tea and Rathinaswamy, Manoj K and Dalwadi, Udit and Yip, Calvin
-K and Burke, John E and Garcia, K. Christopher and Grishin, Nick V. and Adams,
-Paul D. and Read, Randy J. and Baker, David}, title = {Accurate prediction of
-protein structures and interactions using a 3-track network}, year = {2021},
-doi = {10.1101/2021.06.14.448402}, publisher = {Cold Spring Harbor Laboratory},
-URL = {https://www.biorxiv.org/content/early/2021/06/15/2021.06.14.448402},
-eprint = {https://www.biorxiv.org/content/early/2021/06/15/
-2021.06.14.448402.full.pdf}, journal = {bioRxiv} } ``` ```bibtex @misc
-{shi2021masked, title = {Masked Label Prediction: Unified Message Passing Model
-for Semi-Supervised Classification}, author = {Yunsheng Shi and Zhengjie Huang
-and Shikun Feng and Hui Zhong and Wenjin Wang and Yu Sun}, year = {2021},
-eprint = {2009.03509}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ```
+for coordinates ``` If you want it to handle an adjacency matrix ```python
+import torch from graph_transformer_pytorch import GraphTransformer model =
+GraphTransformer( dim = 256, depth = 6, edge_dim = 512, with_feedforwards =
+True, gated_residual = True, rel_pos_emb = True, accept_adjacency_matrix = True
+# set this to True ) nodes = torch.randn(2, 128, 256) adj_mat = torch.randint
+(0, 2, (2, 128, 128)) mask = torch.ones(2, 128).bool() nodes, edges = model
+(nodes, adj_mat = adj_mat, mask = mask) nodes.shape # (1, 128, 256) - project
+to R^3 for coordinates ``` ## Citations ```bibtex @article
+{Costa2021.06.02.446809, author = {Costa, Allan and Ponnapati, Manvitha and
+Jacobson, Joseph M. and Chatterjee, Pranam}, title = {Distillation of MSA
+Embeddings to Folded Protein Structures with Graph Transformers}, year =
+{2021}, doi = {10.1101/2021.06.02.446809}, publisher = {Cold Spring Harbor
+Laboratory}, URL = {https://www.biorxiv.org/content/early/2021/06/02/
+2021.06.02.446809}, eprint = {https://www.biorxiv.org/content/early/2021/06/02/
+2021.06.02.446809.full.pdf}, journal = {bioRxiv} } ``` ```bibtex @article
+{Baek2021.06.14.448402, author = {Baek, Minkyung and DiMaio, Frank and
+Anishchenko, Ivan and Dauparas, Justas and Ovchinnikov, Sergey and Lee, Gyu Rie
+and Wang, Jue and Cong, Qian and Kinch, Lisa N. and Schaeffer, R. Dustin and
+Mill{\'a}n, Claudia and Park, Hahnbeom and Adams, Carson and Glassman, Caleb R.
+and DeGiovanni, Andy and Pereira, Jose H. and Rodrigues, Andria V. and van
+Dijk, Alberdina A. and Ebrecht, Ana C. and Opperman, Diederik J. and
+Sagmeister, Theo and Buhlheller, Christoph and Pavkov-Keller, Tea and
+Rathinaswamy, Manoj K and Dalwadi, Udit and Yip, Calvin K and Burke, John E and
+Garcia, K. Christopher and Grishin, Nick V. and Adams, Paul D. and Read, Randy
+J. and Baker, David}, title = {Accurate prediction of protein structures and
+interactions using a 3-track network}, year = {2021}, doi = {10.1101/
+2021.06.14.448402}, publisher = {Cold Spring Harbor Laboratory}, URL = {https:/
+/www.biorxiv.org/content/early/2021/06/15/2021.06.14.448402}, eprint = {https:/
+/www.biorxiv.org/content/early/2021/06/15/2021.06.14.448402.full.pdf}, journal
+= {bioRxiv} } ``` ```bibtex @misc{shi2021masked, title = {Masked Label
+Prediction: Unified Message Passing Model for Semi-Supervised Classification},
+author = {Yunsheng Shi and Zhengjie Huang and Shikun Feng and Hui Zhong and
+Wenjin Wang and Yu Sun}, year = {2021}, eprint = {2009.03509}, archivePrefix =
+{arXiv}, primaryClass = {cs.LG} } ```
```

### Comparing `graph-transformer-pytorch-0.0.3/graph_transformer_pytorch/graph_transformer_pytorch.py` & `graph-transformer-pytorch-0.1.1/graph_transformer_pytorch/graph_transformer_pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,40 +128,59 @@
         depth,
         dim_head = 64,
         edge_dim = None,
         heads = 8,
         gated_residual = True,
         with_feedforwards = False,
         norm_edges = False,
-        rel_pos_emb = False
+        rel_pos_emb = False,
+        accept_adjacency_matrix = False
     ):
         super().__init__()
         self.layers = List([])
         edge_dim = default(edge_dim, dim)
         self.norm_edges = nn.LayerNorm(edge_dim) if norm_edges else nn.Identity()
 
+        self.adj_emb = nn.Embedding(2, edge_dim) if accept_adjacency_matrix else None
+
         pos_emb = RotaryEmbedding(dim_head) if rel_pos_emb else None
 
         for _ in range(depth):
             self.layers.append(List([
                 List([
                     PreNorm(dim, Attention(dim, pos_emb = pos_emb, edge_dim = edge_dim, dim_head = dim_head, heads = heads)),
                     GatedResidual(dim)
                 ]),
                 List([
                     PreNorm(dim, FeedForward(dim)),
                     GatedResidual(dim)
                 ]) if with_feedforwards else None
             ]))
 
-    def forward(self, nodes, edges, mask = None):
-        edges = self.norm_edges(edges)
+    def forward(
+        self,
+        nodes,
+        edges = None,
+        adj_mat = None,
+        mask = None
+    ):
+        batch, seq, _ = nodes.shape
+
+        if exists(edges):
+            edges = self.norm_edges(edges)
+
+        if exists(adj_mat):
+            assert adj_mat.shape == (batch, seq, seq)
+            assert exists(self.adj_emb), 'accept_adjacency_matrix must be set to True'
+            adj_mat = self.adj_emb(adj_mat.long())
+
+        all_edges = default(edges, 0) + default(adj_mat, 0)
 
         for attn_block, ff_block in self.layers:
             attn, attn_residual = attn_block
-            nodes = attn_residual(attn(nodes, edges, mask = mask), nodes)
+            nodes = attn_residual(attn(nodes, all_edges, mask = mask), nodes)
 
             if exists(ff_block):
                 ff, ff_residual = ff_block
                 nodes = ff_residual(ff(nodes), nodes)
 
         return nodes, edges
```

### Comparing `graph-transformer-pytorch-0.0.3/graph_transformer_pytorch.egg-info/PKG-INFO` & `graph-transformer-pytorch-0.1.1/graph_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: graph-transformer-pytorch
-Version: 0.0.3
+Version: 0.1.1
 Summary: Graph Transformer - Pytorch
 Home-page: https://github.com/lucidrains/graph-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,graphs
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `graph-transformer-pytorch-0.0.3/setup.py` & `graph-transformer-pytorch-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'graph-transformer-pytorch',
   packages = find_packages(),
-  version = '0.0.3',
+  version = '0.1.1',
   license='MIT',
   description = 'Graph Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/graph-transformer-pytorch',
+  long_description_content_type = 'text/markdown',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'transformers',
     'graphs'
   ],
   install_requires=[
```

