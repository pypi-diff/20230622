# Comparing `tmp/pipeline_viz-0.1.1.tar.gz` & `tmp/pipeline_viz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_viz-0.1.1.tar", last modified: Thu Jun 22 05:36:13 2023, max compression
+gzip compressed data, was "pipeline_viz-0.1.2.tar", last modified: Thu Jun 22 05:44:33 2023, max compression
```

## Comparing `pipeline_viz-0.1.1.tar` & `pipeline_viz-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.712960 pipeline_viz-0.1.1/
--rw-r--r--   0 priti      (501) staff       (20)     1068 2023-06-21 21:56:09.000000 pipeline_viz-0.1.1/LICENSE
--rw-r--r--   0 priti      (501) staff       (20)     3116 2023-06-22 05:36:13.712499 pipeline_viz-0.1.1/PKG-INFO
--rw-r--r--   0 priti      (501) staff       (20)     2784 2023-06-22 05:31:27.000000 pipeline_viz-0.1.1/README.md
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.701622 pipeline_viz-0.1.1/pipeline_viz/
--rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:17:34.000000 pipeline_viz-0.1.1/pipeline_viz/__init__.py
--rw-r--r--   0 priti      (501) staff       (20)     8142 2023-06-22 04:50:51.000000 pipeline_viz-0.1.1/pipeline_viz/pipeline_viz.py
--rw-r--r--   0 priti      (501) staff       (20)      454 2023-06-21 21:17:24.000000 pipeline_viz-0.1.1/pipeline_viz/utils.py
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.706110 pipeline_viz-0.1.1/pipeline_viz.egg-info/
--rw-r--r--   0 priti      (501) staff       (20)     3116 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/PKG-INFO
--rw-r--r--   0 priti      (501) staff       (20)      349 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/SOURCES.txt
--rw-r--r--   0 priti      (501) staff       (20)        1 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/dependency_links.txt
--rw-r--r--   0 priti      (501) staff       (20)       46 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/requires.txt
--rw-r--r--   0 priti      (501) staff       (20)       19 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/top_level.txt
--rw-r--r--   0 priti      (501) staff       (20)       38 2023-06-22 05:36:13.713119 pipeline_viz-0.1.1/setup.cfg
--rw-r--r--   0 priti      (501) staff       (20)      593 2023-06-22 05:31:52.000000 pipeline_viz-0.1.1/setup.py
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.709816 pipeline_viz-0.1.1/tests/
--rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:42:27.000000 pipeline_viz-0.1.1/tests/__init__.py
--rw-r--r--   0 priti      (501) staff       (20)     1189 2023-06-22 04:48:12.000000 pipeline_viz-0.1.1/tests/pipeline_test.py
--rw-r--r--   0 priti      (501) staff       (20)     1342 2023-06-21 21:17:20.000000 pipeline_viz-0.1.1/tests/test_pipeline_viz.py
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:44:33.434804 pipeline_viz-0.1.2/
+-rw-r--r--   0 priti      (501) staff       (20)     1068 2023-06-21 21:56:09.000000 pipeline_viz-0.1.2/LICENSE
+-rw-r--r--   0 priti      (501) staff       (20)     3096 2023-06-22 05:44:33.432893 pipeline_viz-0.1.2/PKG-INFO
+-rw-r--r--   0 priti      (501) staff       (20)     2764 2023-06-22 05:39:34.000000 pipeline_viz-0.1.2/README.md
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:44:33.421853 pipeline_viz-0.1.2/pipeline_viz/
+-rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:17:34.000000 pipeline_viz-0.1.2/pipeline_viz/__init__.py
+-rw-r--r--   0 priti      (501) staff       (20)     8142 2023-06-22 04:50:51.000000 pipeline_viz-0.1.2/pipeline_viz/pipeline_viz.py
+-rw-r--r--   0 priti      (501) staff       (20)      454 2023-06-21 21:17:24.000000 pipeline_viz-0.1.2/pipeline_viz/utils.py
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:44:33.428096 pipeline_viz-0.1.2/pipeline_viz.egg-info/
+-rw-r--r--   0 priti      (501) staff       (20)     3096 2023-06-22 05:44:33.000000 pipeline_viz-0.1.2/pipeline_viz.egg-info/PKG-INFO
+-rw-r--r--   0 priti      (501) staff       (20)      349 2023-06-22 05:44:33.000000 pipeline_viz-0.1.2/pipeline_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 priti      (501) staff       (20)        1 2023-06-22 05:44:33.000000 pipeline_viz-0.1.2/pipeline_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 priti      (501) staff       (20)       46 2023-06-22 05:44:33.000000 pipeline_viz-0.1.2/pipeline_viz.egg-info/requires.txt
+-rw-r--r--   0 priti      (501) staff       (20)       19 2023-06-22 05:44:33.000000 pipeline_viz-0.1.2/pipeline_viz.egg-info/top_level.txt
+-rw-r--r--   0 priti      (501) staff       (20)       38 2023-06-22 05:44:33.435038 pipeline_viz-0.1.2/setup.cfg
+-rw-r--r--   0 priti      (501) staff       (20)      593 2023-06-22 05:42:28.000000 pipeline_viz-0.1.2/setup.py
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:44:33.431404 pipeline_viz-0.1.2/tests/
+-rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:42:27.000000 pipeline_viz-0.1.2/tests/__init__.py
+-rw-r--r--   0 priti      (501) staff       (20)     1189 2023-06-22 04:48:12.000000 pipeline_viz-0.1.2/tests/pipeline_test.py
+-rw-r--r--   0 priti      (501) staff       (20)     1342 2023-06-21 21:17:20.000000 pipeline_viz-0.1.2/tests/test_pipeline_viz.py
```

### Comparing `pipeline_viz-0.1.1/LICENSE` & `pipeline_viz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_viz-0.1.1/PKG-INFO` & `pipeline_viz-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pipeline_viz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Visualization tool for sklearn pipelines
 Home-page: https://github.com/pritiyadav888/visualize_pipeline.git
 Author: Pritii Yadav
 Author-email: pritiyadav888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# visualize_pipeline
+
 A Python package that provides a convenient way to visualize Scikit-learn machine learning pipelines. It utilizes libraries such as NetworkX, Matplotlib, and Plotly to generate clear, interactive, and insightful visual representations of your ML pipelines
 
 ## Installation
 
 You can install Visualize Pipeline using pip:
 
 ```python
```

### Comparing `pipeline_viz-0.1.1/README.md` & `pipeline_viz-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# visualize_pipeline
+
 A Python package that provides a convenient way to visualize Scikit-learn machine learning pipelines. It utilizes libraries such as NetworkX, Matplotlib, and Plotly to generate clear, interactive, and insightful visual representations of your ML pipelines
 
 ## Installation
 
 You can install Visualize Pipeline using pip:
 
 ```python
```

### Comparing `pipeline_viz-0.1.1/pipeline_viz/pipeline_viz.py` & `pipeline_viz-0.1.2/pipeline_viz/pipeline_viz.py`

 * *Files identical despite different names*

### Comparing `pipeline_viz-0.1.1/pipeline_viz.egg-info/PKG-INFO` & `pipeline_viz-0.1.2/pipeline_viz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pipeline-viz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Visualization tool for sklearn pipelines
 Home-page: https://github.com/pritiyadav888/visualize_pipeline.git
 Author: Pritii Yadav
 Author-email: pritiyadav888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# visualize_pipeline
+
 A Python package that provides a convenient way to visualize Scikit-learn machine learning pipelines. It utilizes libraries such as NetworkX, Matplotlib, and Plotly to generate clear, interactive, and insightful visual representations of your ML pipelines
 
 ## Installation
 
 You can install Visualize Pipeline using pip:
 
 ```python
```

### Comparing `pipeline_viz-0.1.1/setup.py` & `pipeline_viz-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pipeline_viz',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/pritiyadav888/visualize_pipeline.git',
     author='Pritii Yadav',
     author_email='pritiyadav888@gmail.com',
     description='Visualization tool for sklearn pipelines',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `pipeline_viz-0.1.1/tests/pipeline_test.py` & `pipeline_viz-0.1.2/tests/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `pipeline_viz-0.1.1/tests/test_pipeline_viz.py` & `pipeline_viz-0.1.2/tests/test_pipeline_viz.py`

 * *Files identical despite different names*

