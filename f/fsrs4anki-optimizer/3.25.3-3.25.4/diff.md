# Comparing `tmp/fsrs4anki_optimizer-3.25.3.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.3.tar", last modified: Mon Jun 19 07:13:50 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.4.tar", last modified: Thu Jun 22 06:42:16 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.3.tar` & `fsrs4anki_optimizer-3.25.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:50.435204 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44249 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 07:13:50.000000 fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:13:50.439204 fsrs4anki_optimizer-3.25.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 07:13:36.000000 fsrs4anki_optimizer-3.25.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44545 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,16 +563,16 @@
                 self.difficulty_distribution_padding[i] = self.difficulty_distribution.loc[i+1]
         return self.difficulty_distribution
     
     def find_optimal_retention(self):
         """should not be called before predict_memory_states"""
 
         base = 1.01
-        index_len = 664
-        index_offset = 200
+        minimum_stability = 0.1
+        index_offset = -(np.log(minimum_stability) / np.log(base)).round().astype(int)
         d_range = 10
         d_offset = 1
         r_time = 8
         f_time = 25
         max_time = 1e10
 
         type_block = dict()
@@ -605,15 +605,18 @@
 
         def cal_next_recall_stability(s, r, d, response):
             if response == 1:
                 return s * (1 + np.exp(self.w[6]) * (11 - d) * np.power(s, self.w[7]) * (np.exp((1 - r) * self.w[8]) - 1))
             else:
                 return self.w[9] * np.power(d, self.w[10]) * np.power(s, self.w[11]) * np.exp((1 - r) * self.w[12])
 
-
+        terminal_stability = minimum_stability
+        for _ in range(128):
+            terminal_stability = cal_next_recall_stability(terminal_stability, 0.96, d_range, 1)
+        index_len = stability2index(terminal_stability)
         stability_list = np.array([np.power(base, i - index_offset) for i in range(index_len)])
         print(f"terminal stability: {stability_list.max(): .2f}")
         df = pd.DataFrame(columns=["retention", "difficulty", "time"])
 
         for percentage in tqdm(range(96, 66, -2), desc="find optimal retention"):
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
```

