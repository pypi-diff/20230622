# Comparing `tmp/grad-info-opt-0.1.1.tar.gz` & `tmp/grad-info-opt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grad-info-opt-0.1.1.tar", last modified: Wed May 17 18:26:19 2023, max compression
+gzip compressed data, was "grad-info-opt-0.1.2.tar", last modified: Thu Jun 22 18:39:05 2023, max compression
```

## Comparing `grad-info-opt-0.1.1.tar` & `grad-info-opt-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:19.150992 grad-info-opt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-17 18:26:19.146992 grad-info-opt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:26:19.150992 grad-info-opt-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:19.146992 grad-info-opt-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:19.146992 grad-info-opt-0.1.1/src/GIO/
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/src/GIO/GIOKL.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/src/GIO/GIO_super.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/src/GIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 18:26:04.000000 grad-info-opt-0.1.1/src/GIO/generate_text_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:19.146992 grad-info-opt-0.1.1/src/grad_info_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-17 18:26:19.000000 grad-info-opt-0.1.1/src/grad_info_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 18:26:19.000000 grad-info-opt-0.1.1/src/grad_info_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:26:19.000000 grad-info-opt-0.1.1/src/grad_info_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 18:26:19.000000 grad-info-opt-0.1.1/src/grad_info_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 18:26:19.000000 grad-info-opt-0.1.1/src/grad_info_opt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:39:05.205231 grad-info-opt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-22 18:39:05.205231 grad-info-opt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:39:05.205231 grad-info-opt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:39:05.201231 grad-info-opt-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:39:05.205231 grad-info-opt-0.1.2/src/GIO/
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/src/GIO/GIOKL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/src/GIO/GIO_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/src/GIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 18:38:53.000000 grad-info-opt-0.1.2/src/GIO/generate_text_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:39:05.205231 grad-info-opt-0.1.2/src/grad_info_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-22 18:39:05.000000 grad-info-opt-0.1.2/src/grad_info_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 18:39:05.000000 grad-info-opt-0.1.2/src/grad_info_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:39:05.000000 grad-info-opt-0.1.2/src/grad_info_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 18:39:05.000000 grad-info-opt-0.1.2/src/grad_info_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 18:39:05.000000 grad-info-opt-0.1.2/src/grad_info_opt.egg-info/top_level.txt
```

### Comparing `grad-info-opt-0.1.1/LICENSE` & `grad-info-opt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grad-info-opt-0.1.1/PKG-INFO` & `grad-info-opt-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-Metadata-Version: 2.1
-Name: grad-info-opt
-Version: 0.1.1
-Summary: Implementation of Gradient Information Optimization for efficient and scalable training data selection
-Home-page: https://github.com/daeveraert/gradient-information-optimization
-Author: Dante Everaert
-Author-email: dante.everaert@berkeley.edu
-Project-URL: Bug Tracker, https://github.com/daeveraert/gradient-information-optimization/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GIO: Gradient Information Optimization
 <p align="center">
   <img alt="" src="https://github.com/daeveraert/gradient-information-optimization/blob/main/images/process.gif">
 </p>
 
-GIO is a library that implements Gradient Information Optimization (GIO) at scale. GIO is a data selection technique that can
+GIO is a library that implements Gradient Information Optimization (GIO) at scale, from the paper <a href=https://arxiv.org/abs/2306.11670>GIO: Gradient Information Optimization for Training Dataset Selection</a>. GIO is a data selection technique that can
 be used to select a subset of training data that gives similar or superior performance to a model trained on full data.
 
+**Paper Abstract**
+
+It is often advantageous to train models on a subset of the available train examples, because the examples are of variable quality or because one would like to train with fewer examples, without sacrificing performance. We present Gradient Information Optimization (GIO), a scalable, task-agnostic approach to this data selection problem that requires only a small set of (unlabeled) examples representing a target distribution. GIO begins from a natural, information-theoretic objective that is intractable in practice. Our contribution is in showing that it can be made highly scalable through a simple relaxation of the objective and a highly efficient implementation. In experiments with machine translation, spelling correction, and image recognition, we show that GIO delivers outstanding results with very small train sets. These findings are robust to different representation models and hyperparameters for GIO itself. GIO is task- and domain-agnostic and can be applied out-of-the-box to new datasets and domains.
+
+
 **Features**:
 - GIO with quantization using K-means.
 - Sentence embedding script to generate embeddings from data to use in GIO
 
+
 ## Installation
 
 Installable via pip:
 ```bash
 pip install grad-info-opt
 ``` 
 Or install directly form the repository:
@@ -42,15 +33,15 @@
 Direct installation will require you to install additional dependencies listed below. We welcome contributions to GIO.
 
 ## Requirements
 - `numpy>=1.21.6`
 - `jax>=0.3.25`
 - `pyspark>=2.4.8`
 - `sentence_transformers>=2.2.2`
-- `jaxlib>=0.4.7`
+- `jaxlib>=0.3.2`
 - `pandas>=1.0.5`
 
 
 
 ## Quick Start
 **Note:** GIO uses a Spark context, or if it can't find one, it will create a local one. You may encounter a Spark error before the algorithm runs complaining it cannot find a free port. In this case, executing ```export SPARK_LOCAL_IP="127.0.0.1"``` should resolve the issue.
 
@@ -127,26 +118,26 @@
 centroids_df = gio_kl.spark.createDataFrame(data=[(i, each.tolist()) for i, each in enumerate(model_train.clusterCenters())], schema=["id", "centroid"])
 
 # Perform the Algorithm
 W, kl_divs, _ = gio_kl.fit(train, X, max_iter=300, stopping_criterion='sequential_increase_tolerance', v_init='jump')
 W = W[20:] # Remove the uniform start
 
 # Explode back to original data and write resulting data
-full_selections_df = gio_kl.explode(W, centroids_df, transformed_train)
+full_selections_df = gio_kl.explode(W, transformed_train, centroids_df)
 full_selections_df.select(F.col("_c0"), F.col("_c1")).write.option("delimiter", "\t").csv(OUTPUT_PATH)
 
 
 # Plot results
 plt.plot(kl_divs)
 plt.title("KL Divergence vs. Iterations")
 plt.xlabel("Iterations")
 plt.ylabel("KL Divergence")
 plt.show()
 ```
-
+**Note:** For quantization, Spark requires a large rpc message size. It is recommended to place ```gio_kl.spark.conf.set("spark.rpc.message.maxSize", "500")```  (or any large number) in the code before calling quantize, if the defaults haven't already been increased.
 
 ## Available Options
 `GIOKL.fit` takes the following arguments:
 - `train`: training data as a jnp array (jnp is almost identical to numpy) [M, D] shape
 - `X`: target data as a jnp array [N, D] shape
 - `D`: initial data as a jnp array, default None. Use None to initialize from 0 (uniform) or a subset of training data
 - `k`: kth nearest neighbor to use in the KL divergence estimation, default 5
@@ -163,18 +154,18 @@
 - `scale_factor`: factor to scale the gradient by, or 'auto'. Default is 'auto', which is recommended
 - `v_init`: how to initialize v in gradients descent, one of the following: 'mean', 'prev_opt', 'jump'. Default is 'mean'
 - `grad_desc_iter`: the number of iterations to use in gradient descent. Default is 50
 - `discard_nearest_for_xy`: discard nearest in the xy calculation of KL divergence, for use when X and the train set are the same, comes at the cost of efficiency. Default is False
 - `lr`: Learning rate for gradient descent. Default is 0.01
 
 ## Citing GIO
-If you use GIO in a publication or blog, please cite this software.
+If you use GIO in a publication, blog or software project, please cite the paper:
 ```
-@software{gradient-information-optimization,
-  author = {Dante Everaert},
-  title = {GIO: Gradient Information Optimization for Training Dataset Selection},
-  url = {https://github.com/daeveraert/gradient-information-optimization},
-  version = {0.1.0},
-  year = {2023},
-  note = {Apache 2.0 License}
+@misc{everaert2023gio,
+      title={GIO: Gradient Information Optimization for Training Dataset Selection}, 
+      author={Dante Everaert and Christopher Potts},
+      year={2023},
+      eprint={2306.11670},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
 }
 ```
```

### Comparing `grad-info-opt-0.1.1/README.md` & `grad-info-opt-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,40 @@
+Metadata-Version: 2.1
+Name: grad-info-opt
+Version: 0.1.2
+Summary: Implementation of Gradient Information Optimization for efficient and scalable training data selection
+Home-page: https://github.com/daeveraert/gradient-information-optimization
+Author: Dante Everaert
+Author-email: dante.everaert@berkeley.edu
+Project-URL: Bug Tracker, https://github.com/daeveraert/gradient-information-optimization/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GIO: Gradient Information Optimization
 <p align="center">
   <img alt="" src="https://github.com/daeveraert/gradient-information-optimization/blob/main/images/process.gif">
 </p>
 
-GIO is a library that implements Gradient Information Optimization (GIO) at scale. GIO is a data selection technique that can
+GIO is a library that implements Gradient Information Optimization (GIO) at scale, from the paper <a href=https://arxiv.org/abs/2306.11670>GIO: Gradient Information Optimization for Training Dataset Selection</a>. GIO is a data selection technique that can
 be used to select a subset of training data that gives similar or superior performance to a model trained on full data.
 
+**Paper Abstract**
+
+It is often advantageous to train models on a subset of the available train examples, because the examples are of variable quality or because one would like to train with fewer examples, without sacrificing performance. We present Gradient Information Optimization (GIO), a scalable, task-agnostic approach to this data selection problem that requires only a small set of (unlabeled) examples representing a target distribution. GIO begins from a natural, information-theoretic objective that is intractable in practice. Our contribution is in showing that it can be made highly scalable through a simple relaxation of the objective and a highly efficient implementation. In experiments with machine translation, spelling correction, and image recognition, we show that GIO delivers outstanding results with very small train sets. These findings are robust to different representation models and hyperparameters for GIO itself. GIO is task- and domain-agnostic and can be applied out-of-the-box to new datasets and domains.
+
+
 **Features**:
 - GIO with quantization using K-means.
 - Sentence embedding script to generate embeddings from data to use in GIO
 
+
 ## Installation
 
 Installable via pip:
 ```bash
 pip install grad-info-opt
 ``` 
 Or install directly form the repository:
@@ -27,15 +48,15 @@
 Direct installation will require you to install additional dependencies listed below. We welcome contributions to GIO.
 
 ## Requirements
 - `numpy>=1.21.6`
 - `jax>=0.3.25`
 - `pyspark>=2.4.8`
 - `sentence_transformers>=2.2.2`
-- `jaxlib>=0.4.7`
+- `jaxlib>=0.3.2`
 - `pandas>=1.0.5`
 
 
 
 ## Quick Start
 **Note:** GIO uses a Spark context, or if it can't find one, it will create a local one. You may encounter a Spark error before the algorithm runs complaining it cannot find a free port. In this case, executing ```export SPARK_LOCAL_IP="127.0.0.1"``` should resolve the issue.
 
@@ -112,26 +133,26 @@
 centroids_df = gio_kl.spark.createDataFrame(data=[(i, each.tolist()) for i, each in enumerate(model_train.clusterCenters())], schema=["id", "centroid"])
 
 # Perform the Algorithm
 W, kl_divs, _ = gio_kl.fit(train, X, max_iter=300, stopping_criterion='sequential_increase_tolerance', v_init='jump')
 W = W[20:] # Remove the uniform start
 
 # Explode back to original data and write resulting data
-full_selections_df = gio_kl.explode(W, centroids_df, transformed_train)
+full_selections_df = gio_kl.explode(W, transformed_train, centroids_df)
 full_selections_df.select(F.col("_c0"), F.col("_c1")).write.option("delimiter", "\t").csv(OUTPUT_PATH)
 
 
 # Plot results
 plt.plot(kl_divs)
 plt.title("KL Divergence vs. Iterations")
 plt.xlabel("Iterations")
 plt.ylabel("KL Divergence")
 plt.show()
 ```
-
+**Note:** For quantization, Spark requires a large rpc message size. It is recommended to place ```gio_kl.spark.conf.set("spark.rpc.message.maxSize", "500")```  (or any large number) in the code before calling quantize, if the defaults haven't already been increased.
 
 ## Available Options
 `GIOKL.fit` takes the following arguments:
 - `train`: training data as a jnp array (jnp is almost identical to numpy) [M, D] shape
 - `X`: target data as a jnp array [N, D] shape
 - `D`: initial data as a jnp array, default None. Use None to initialize from 0 (uniform) or a subset of training data
 - `k`: kth nearest neighbor to use in the KL divergence estimation, default 5
@@ -148,18 +169,18 @@
 - `scale_factor`: factor to scale the gradient by, or 'auto'. Default is 'auto', which is recommended
 - `v_init`: how to initialize v in gradients descent, one of the following: 'mean', 'prev_opt', 'jump'. Default is 'mean'
 - `grad_desc_iter`: the number of iterations to use in gradient descent. Default is 50
 - `discard_nearest_for_xy`: discard nearest in the xy calculation of KL divergence, for use when X and the train set are the same, comes at the cost of efficiency. Default is False
 - `lr`: Learning rate for gradient descent. Default is 0.01
 
 ## Citing GIO
-If you use GIO in a publication or blog, please cite this software.
+If you use GIO in a publication, blog or software project, please cite the paper:
 ```
-@software{gradient-information-optimization,
-  author = {Dante Everaert},
-  title = {GIO: Gradient Information Optimization for Training Dataset Selection},
-  url = {https://github.com/daeveraert/gradient-information-optimization},
-  version = {0.1.0},
-  year = {2023},
-  note = {Apache 2.0 License}
+@misc{everaert2023gio,
+      title={GIO: Gradient Information Optimization for Training Dataset Selection}, 
+      author={Dante Everaert and Christopher Potts},
+      year={2023},
+      eprint={2306.11670},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
 }
 ```
```

### Comparing `grad-info-opt-0.1.1/setup.py` & `grad-info-opt-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="grad-info-opt",
-    version="0.1.1",
+    version="0.1.2",
     author="Dante Everaert",
     author_email="dante.everaert@berkeley.edu",
     description="Implementation of Gradient Information Optimization for efficient and scalable training data selection",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/daeveraert/gradient-information-optimization",
     project_urls={
@@ -24,10 +24,10 @@
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
         'jax>=0.3.25',
         'pyspark>=2.4.8',
         'numpy>=1.21.6',
         'sentence_transformers>=2.2.2',
-        'jaxlib>=0.4.7',
+        'jaxlib>=0.3.2',
         'pandas>=1.0.5']
 )
```

### Comparing `grad-info-opt-0.1.1/src/GIO/GIOKL.py` & `grad-info-opt-0.1.2/src/GIO/GIOKL.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,17 @@
         just_reset = False
         num_resets = 0
         total_iter = 0
         increases = 0
         while True:
             # Warmup, reset or random restart
             if i == 0 or just_reset or random.random() < random_restart_prob:
-                v = self.gradient_descend(X, W, v, scale_factor, grad_desc_iter * 3, lr=lr, k=k)
+                v = self.gradient_descend(X, W, v, scale_factor, grad_desc_iter * 3, lr=lr, k=k, discard_nearest_for_xy=discard_nearest_for_xy)
             else:
-                v = self.gradient_descend(X, W, v, scale_factor, grad_desc_iter, lr=lr, k=k)
+                v = self.gradient_descend(X, W, v, scale_factor, grad_desc_iter, lr=lr, k=k, discard_nearest_for_xy=discard_nearest_for_xy)
             idx = self._get_nearest(v, adder)
             minvals = adder[idx]
             adder = jnp.delete(adder, idx, axis=0)
 
             W_tmp = jnp.concatenate((W, jnp.array(minvals)[jnp.newaxis, :]))
 
             kl_dist = self.calculate_statistical_distance(X, W_tmp, k, discard_nearest_for_xy=discard_nearest_for_xy)
@@ -191,15 +191,15 @@
                 break
 
             if v_init == 'mean':
                 v = jnp.mean(X, axis=0)
             elif v_init == 'jump':
                 v = jnp.array(random.sample(X.tolist(), 1)).squeeze()
 
-            adder, i, just_reset, stop, v, increases = self._test_stop_criterion(v_init, stop_criterion, kl_dist, kl_dist_prev, num_resets, max_resets, min_difference, increases, max_sequential_increases, min_kl, max_data_size, train, X, i, v, just_reset, resets_allowed, adder)
+            adder, i, just_reset, stop, v, increases, num_resets = self._test_stop_criterion(v_init, stop_criterion, kl_dist, kl_dist_prev, num_resets, max_resets, min_difference, increases, max_sequential_increases, min_kl, max_data_size, train, X, i, v, just_reset, resets_allowed, adder)
 
             if stop:
                 break
             if not just_reset:
                 W = W_tmp
                 kl_divs += [kl_dist]
                 kl_dist_prev = kl_dist
@@ -232,15 +232,15 @@
                 adder = train[:]
                 i -= 1
                 stop = False
             just_reset = True
         else:
             just_reset = False
             increases = 0
-        return adder, i, just_reset, stop, v, increases
+        return adder, i, just_reset, stop, v, increases, num_resets
 
     def _return_kmeans(self, df, k, rseed):
         """Use Spark to perform K-Means
         :param df: dataframe to perform K-Means with
         :param k: number of clusters to compute
         :param rseed: random seed
         :return: k-means model, transformed df
@@ -289,16 +289,19 @@
     def read_data_from_parquet(self, path, path_X):
         """Read in and process data stored in a parquet format. Data must contain a column "features" that stores an array<double>
         of the vectors and be non-nullable.
         :param path: path to training data
         :param path_X: path to target data
         :return: train df, target df
         """
-        df_with_embeddings = self.spark.read.parquet(path)
-        df_X_with_embeddings = self.spark.read.parquet(path_X)
+        new_schema = ArrayType(DoubleType(), containsNull=False)
+        udf_no_null = F.udf(lambda x: x, new_schema)
+
+        df_with_embeddings = self.spark.read.parquet(path).withColumn("features", udf_no_null(F.col("features")))
+        df_X_with_embeddings = self.spark.read.parquet(path_X).withColumn("features", udf_no_null(F.col("features")))
         return df_with_embeddings, df_X_with_embeddings
 
     def explode(self, chosen_centroids, kmeans_transformed_df, kmeans_centroids_df):
         """Read in and process data stored in a parquet format. Data must contain a column "features" that stores an array<double>
         of the vectors.
         :param path: path to training data
         :param path_X: path to target data
```

### Comparing `grad-info-opt-0.1.1/src/GIO/GIO_super.py` & `grad-info-opt-0.1.2/src/GIO/GIO_super.py`

 * *Files identical despite different names*

### Comparing `grad-info-opt-0.1.1/src/GIO/generate_text_embeddings.py` & `grad-info-opt-0.1.2/src/GIO/generate_text_embeddings.py`

 * *Files identical despite different names*

### Comparing `grad-info-opt-0.1.1/src/grad_info_opt.egg-info/PKG-INFO` & `grad-info-opt-0.1.2/src/grad_info_opt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-info-opt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of Gradient Information Optimization for efficient and scalable training data selection
 Home-page: https://github.com/daeveraert/gradient-information-optimization
 Author: Dante Everaert
 Author-email: dante.everaert@berkeley.edu
 Project-URL: Bug Tracker, https://github.com/daeveraert/gradient-information-optimization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,21 +14,27 @@
 License-File: LICENSE
 
 # GIO: Gradient Information Optimization
 <p align="center">
   <img alt="" src="https://github.com/daeveraert/gradient-information-optimization/blob/main/images/process.gif">
 </p>
 
-GIO is a library that implements Gradient Information Optimization (GIO) at scale. GIO is a data selection technique that can
+GIO is a library that implements Gradient Information Optimization (GIO) at scale, from the paper <a href=https://arxiv.org/abs/2306.11670>GIO: Gradient Information Optimization for Training Dataset Selection</a>. GIO is a data selection technique that can
 be used to select a subset of training data that gives similar or superior performance to a model trained on full data.
 
+**Paper Abstract**
+
+It is often advantageous to train models on a subset of the available train examples, because the examples are of variable quality or because one would like to train with fewer examples, without sacrificing performance. We present Gradient Information Optimization (GIO), a scalable, task-agnostic approach to this data selection problem that requires only a small set of (unlabeled) examples representing a target distribution. GIO begins from a natural, information-theoretic objective that is intractable in practice. Our contribution is in showing that it can be made highly scalable through a simple relaxation of the objective and a highly efficient implementation. In experiments with machine translation, spelling correction, and image recognition, we show that GIO delivers outstanding results with very small train sets. These findings are robust to different representation models and hyperparameters for GIO itself. GIO is task- and domain-agnostic and can be applied out-of-the-box to new datasets and domains.
+
+
 **Features**:
 - GIO with quantization using K-means.
 - Sentence embedding script to generate embeddings from data to use in GIO
 
+
 ## Installation
 
 Installable via pip:
 ```bash
 pip install grad-info-opt
 ``` 
 Or install directly form the repository:
@@ -42,15 +48,15 @@
 Direct installation will require you to install additional dependencies listed below. We welcome contributions to GIO.
 
 ## Requirements
 - `numpy>=1.21.6`
 - `jax>=0.3.25`
 - `pyspark>=2.4.8`
 - `sentence_transformers>=2.2.2`
-- `jaxlib>=0.4.7`
+- `jaxlib>=0.3.2`
 - `pandas>=1.0.5`
 
 
 
 ## Quick Start
 **Note:** GIO uses a Spark context, or if it can't find one, it will create a local one. You may encounter a Spark error before the algorithm runs complaining it cannot find a free port. In this case, executing ```export SPARK_LOCAL_IP="127.0.0.1"``` should resolve the issue.
 
@@ -127,26 +133,26 @@
 centroids_df = gio_kl.spark.createDataFrame(data=[(i, each.tolist()) for i, each in enumerate(model_train.clusterCenters())], schema=["id", "centroid"])
 
 # Perform the Algorithm
 W, kl_divs, _ = gio_kl.fit(train, X, max_iter=300, stopping_criterion='sequential_increase_tolerance', v_init='jump')
 W = W[20:] # Remove the uniform start
 
 # Explode back to original data and write resulting data
-full_selections_df = gio_kl.explode(W, centroids_df, transformed_train)
+full_selections_df = gio_kl.explode(W, transformed_train, centroids_df)
 full_selections_df.select(F.col("_c0"), F.col("_c1")).write.option("delimiter", "\t").csv(OUTPUT_PATH)
 
 
 # Plot results
 plt.plot(kl_divs)
 plt.title("KL Divergence vs. Iterations")
 plt.xlabel("Iterations")
 plt.ylabel("KL Divergence")
 plt.show()
 ```
-
+**Note:** For quantization, Spark requires a large rpc message size. It is recommended to place ```gio_kl.spark.conf.set("spark.rpc.message.maxSize", "500")```  (or any large number) in the code before calling quantize, if the defaults haven't already been increased.
 
 ## Available Options
 `GIOKL.fit` takes the following arguments:
 - `train`: training data as a jnp array (jnp is almost identical to numpy) [M, D] shape
 - `X`: target data as a jnp array [N, D] shape
 - `D`: initial data as a jnp array, default None. Use None to initialize from 0 (uniform) or a subset of training data
 - `k`: kth nearest neighbor to use in the KL divergence estimation, default 5
@@ -163,18 +169,18 @@
 - `scale_factor`: factor to scale the gradient by, or 'auto'. Default is 'auto', which is recommended
 - `v_init`: how to initialize v in gradients descent, one of the following: 'mean', 'prev_opt', 'jump'. Default is 'mean'
 - `grad_desc_iter`: the number of iterations to use in gradient descent. Default is 50
 - `discard_nearest_for_xy`: discard nearest in the xy calculation of KL divergence, for use when X and the train set are the same, comes at the cost of efficiency. Default is False
 - `lr`: Learning rate for gradient descent. Default is 0.01
 
 ## Citing GIO
-If you use GIO in a publication or blog, please cite this software.
+If you use GIO in a publication, blog or software project, please cite the paper:
 ```
-@software{gradient-information-optimization,
-  author = {Dante Everaert},
-  title = {GIO: Gradient Information Optimization for Training Dataset Selection},
-  url = {https://github.com/daeveraert/gradient-information-optimization},
-  version = {0.1.0},
-  year = {2023},
-  note = {Apache 2.0 License}
+@misc{everaert2023gio,
+      title={GIO: Gradient Information Optimization for Training Dataset Selection}, 
+      author={Dante Everaert and Christopher Potts},
+      year={2023},
+      eprint={2306.11670},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
 }
 ```
```

