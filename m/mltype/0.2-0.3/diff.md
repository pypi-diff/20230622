# Comparing `tmp/mltype-0.2.tar.gz` & `tmp/mltype-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltype-0.2.tar", last modified: Wed Mar 23 21:32:43 2022, max compression
+gzip compressed data, was "mltype-0.3.tar", last modified: Thu Jun 22 15:01:22 2023, max compression
```

## Comparing `mltype-0.2.tar` & `mltype-0.3.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 krepl    (1265904033)    10067        0 2022-03-23 21:32:43.404312 mltype-0.2/
--rw-r--r--   0 krepl    (1265904033)    10067     1066 2021-10-11 07:51:10.000000 mltype-0.2/LICENSE
--rw-r--r--   0 krepl    (1265904033)    10067      349 2022-03-23 21:32:43.404191 mltype-0.2/PKG-INFO
--rw-r--r--   0 krepl    (1265904033)    10067     7265 2021-10-11 07:51:10.000000 mltype-0.2/README.md
-drwxr-xr-x   0 krepl    (1265904033)    10067        0 2022-03-23 21:32:43.403273 mltype-0.2/mltype/
--rw-r--r--   0 krepl    (1265904033)    10067       43 2022-03-23 21:23:16.000000 mltype-0.2/mltype/__init__.py
--rw-r--r--   0 krepl    (1265904033)    10067     8018 2021-10-11 07:51:10.000000 mltype-0.2/mltype/base.py
--rw-r--r--   0 krepl    (1265904033)    10067    16184 2021-10-11 07:51:10.000000 mltype-0.2/mltype/cli.py
--rw-r--r--   0 krepl    (1265904033)    10067     1281 2021-10-11 07:51:10.000000 mltype-0.2/mltype/data.py
--rw-r--r--   0 krepl    (1265904033)    10067    14108 2021-10-11 07:51:10.000000 mltype-0.2/mltype/interactive.py
--rw-r--r--   0 krepl    (1265904033)    10067    26733 2021-10-11 07:51:10.000000 mltype-0.2/mltype/ml.py
--rw-r--r--   0 krepl    (1265904033)    10067      768 2021-10-11 07:51:10.000000 mltype-0.2/mltype/stats.py
--rw-r--r--   0 krepl    (1265904033)    10067     3356 2021-10-11 07:51:10.000000 mltype-0.2/mltype/utils.py
-drwxr-xr-x   0 krepl    (1265904033)    10067        0 2022-03-23 21:32:43.404038 mltype-0.2/mltype.egg-info/
--rw-r--r--   0 krepl    (1265904033)    10067      349 2022-03-23 21:32:43.000000 mltype-0.2/mltype.egg-info/PKG-INFO
--rw-r--r--   0 krepl    (1265904033)    10067      338 2022-03-23 21:32:43.000000 mltype-0.2/mltype.egg-info/SOURCES.txt
--rw-r--r--   0 krepl    (1265904033)    10067        1 2022-03-23 21:32:43.000000 mltype-0.2/mltype.egg-info/dependency_links.txt
--rw-r--r--   0 krepl    (1265904033)    10067       40 2022-03-23 21:32:43.000000 mltype-0.2/mltype.egg-info/entry_points.txt
--rw-r--r--   0 krepl    (1265904033)    10067      154 2022-03-23 21:32:43.000000 mltype-0.2/mltype.egg-info/requires.txt
--rw-r--r--   0 krepl    (1265904033)    10067        7 2022-03-23 21:32:43.000000 mltype-0.2/mltype.egg-info/top_level.txt
--rw-r--r--   0 krepl    (1265904033)    10067       38 2022-03-23 21:32:43.404357 mltype-0.2/setup.cfg
--rw-r--r--   0 krepl    (1265904033)    10067      974 2022-03-23 20:34:37.000000 mltype-0.2/setup.py
+drwxr-xr-x   0 krepl    (1265904033)    10067        0 2023-06-22 15:01:22.106242 mltype-0.3/
+-rw-r--r--   0 krepl    (1265904033)    10067     1066 2021-10-11 07:51:10.000000 mltype-0.3/LICENSE
+-rw-r--r--   0 krepl    (1265904033)    10067      330 2023-06-22 15:01:22.106107 mltype-0.3/PKG-INFO
+-rw-r--r--   0 krepl    (1265904033)    10067     7265 2023-06-22 13:55:31.000000 mltype-0.3/README.md
+drwxr-xr-x   0 krepl    (1265904033)    10067        0 2023-06-22 15:01:22.103865 mltype-0.3/mltype/
+-rw-r--r--   0 krepl    (1265904033)    10067       43 2023-06-22 14:57:19.000000 mltype-0.3/mltype/__init__.py
+-rw-r--r--   0 krepl    (1265904033)    10067     8018 2021-10-11 07:51:10.000000 mltype-0.3/mltype/base.py
+-rw-r--r--   0 krepl    (1265904033)    10067    16184 2021-10-11 07:51:10.000000 mltype-0.3/mltype/cli.py
+-rw-r--r--   0 krepl    (1265904033)    10067     1281 2021-10-11 07:51:10.000000 mltype-0.3/mltype/data.py
+-rw-r--r--   0 krepl    (1265904033)    10067    14108 2021-10-11 07:51:10.000000 mltype-0.3/mltype/interactive.py
+-rw-r--r--   0 krepl    (1265904033)    10067    26735 2023-06-22 14:57:07.000000 mltype-0.3/mltype/ml.py
+-rw-r--r--   0 krepl    (1265904033)    10067      768 2021-10-11 07:51:10.000000 mltype-0.3/mltype/stats.py
+-rw-r--r--   0 krepl    (1265904033)    10067     3356 2021-10-11 07:51:10.000000 mltype-0.3/mltype/utils.py
+drwxr-xr-x   0 krepl    (1265904033)    10067        0 2023-06-22 15:01:22.104579 mltype-0.3/mltype.egg-info/
+-rw-r--r--   0 krepl    (1265904033)    10067      330 2023-06-22 15:01:22.000000 mltype-0.3/mltype.egg-info/PKG-INFO
+-rw-r--r--   0 krepl    (1265904033)    10067      477 2023-06-22 15:01:22.000000 mltype-0.3/mltype.egg-info/SOURCES.txt
+-rw-r--r--   0 krepl    (1265904033)    10067        1 2023-06-22 15:01:22.000000 mltype-0.3/mltype.egg-info/dependency_links.txt
+-rw-r--r--   0 krepl    (1265904033)    10067       39 2023-06-22 15:01:22.000000 mltype-0.3/mltype.egg-info/entry_points.txt
+-rw-r--r--   0 krepl    (1265904033)    10067      146 2023-06-22 15:01:22.000000 mltype-0.3/mltype.egg-info/requires.txt
+-rw-r--r--   0 krepl    (1265904033)    10067        7 2023-06-22 15:01:22.000000 mltype-0.3/mltype.egg-info/top_level.txt
+-rw-r--r--   0 krepl    (1265904033)    10067       38 2023-06-22 15:01:22.106283 mltype-0.3/setup.cfg
+-rw-r--r--   0 krepl    (1265904033)    10067      966 2023-06-22 14:57:07.000000 mltype-0.3/setup.py
+drwxr-xr-x   0 krepl    (1265904033)    10067        0 2023-06-22 15:01:22.105858 mltype-0.3/tests/
+-rw-r--r--   0 krepl    (1265904033)    10067     3489 2022-03-23 20:34:37.000000 mltype-0.3/tests/test_base.py
+-rw-r--r--   0 krepl    (1265904033)    10067    21918 2021-10-11 07:51:10.000000 mltype-0.3/tests/test_cli.py
+-rw-r--r--   0 krepl    (1265904033)    10067     1343 2021-10-11 07:51:10.000000 mltype-0.3/tests/test_data.py
+-rw-r--r--   0 krepl    (1265904033)    10067     6724 2023-06-22 14:57:07.000000 mltype-0.3/tests/test_interactive.py
+-rw-r--r--   0 krepl    (1265904033)    10067    12025 2023-06-22 14:57:07.000000 mltype-0.3/tests/test_ml.py
+-rw-r--r--   0 krepl    (1265904033)    10067      606 2021-10-11 07:51:10.000000 mltype-0.3/tests/test_stats.py
+-rw-r--r--   0 krepl    (1265904033)    10067     1502 2021-10-11 07:51:10.000000 mltype-0.3/tests/test_utils.py
```

### Comparing `mltype-0.2/LICENSE` & `mltype-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mltype-0.2/README.md` & `mltype-0.3/README.md`

 * *Files identical despite different names*

### Comparing `mltype-0.2/mltype/base.py` & `mltype-0.3/mltype/base.py`

 * *Files identical despite different names*

### Comparing `mltype-0.2/mltype/cli.py` & `mltype-0.3/mltype/cli.py`

 * *Files identical despite different names*

### Comparing `mltype-0.2/mltype/data.py` & `mltype-0.3/mltype/data.py`

 * *Files identical despite different names*

### Comparing `mltype-0.2/mltype/interactive.py` & `mltype-0.3/mltype/interactive.py`

 * *Files identical despite different names*

### Comparing `mltype-0.2/mltype/ml.py` & `mltype-0.3/mltype/ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         vector.
     """
     text_size = len(text)
     vocab_size = len(vocabulary)
 
     ch2ix = {ch: ix for ix, ch in enumerate(vocabulary)}
 
-    output = np.zeros((text_size, vocab_size), dtype=np.bool)
+    output = np.zeros((text_size, vocab_size), dtype=np.bool_)
     for i, ch in enumerate(text):
         try:
             output[i, ch2ix[ch]] = True
         except KeyError:
             pass
 
     return output
@@ -191,15 +191,15 @@
         A character from the vocabulary.
     """
     device = device or torch.device("cpu")
 
     if previous_chars:
         features = text2features(previous_chars, vocabulary)
     else:
-        features = np.zeros((1, len(vocabulary)), dtype=np.bool)
+        features = np.zeros((1, len(vocabulary)), dtype=np.bool_)
 
     network.eval()
 
     features = features[None, ...]  # add batch dimension
 
     if random_state is not None:
         np.random.seed(random_state)
```

### Comparing `mltype-0.2/mltype/stats.py` & `mltype-0.3/mltype/stats.py`

 * *Files identical despite different names*

### Comparing `mltype-0.2/mltype/utils.py` & `mltype-0.3/mltype/utils.py`

 * *Files identical despite different names*

### Comparing `mltype-0.2/setup.py` & `mltype-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             "black",
             "flake8",
             "pydocstyle",
             "pytest",
             "pytest-coverage",
             "tox",
         ],
-        "mlflow": ["mlflow<=1.10.0"],
+        "mlflow": ["mlflow"],
     },
     entry_points={
         "console_scripts": [
             "mlt = mltype.cli:cli",
         ]
     },
 )
```

