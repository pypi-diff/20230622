# Comparing `tmp/datafog-1.2.0.tar.gz` & `tmp/datafog-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-1.2.0.tar", last modified: Thu Jun 22 17:08:09 2023, max compression
+gzip compressed data, was "dist/datafog-1.3.0.tar", last modified: Thu Jun 22 17:55:46 2023, max compression
```

## Comparing `datafog-1.2.0.tar` & `datafog-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.889904 datafog-1.2.0/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.2.0/LICENSE.MD
--rw-r--r--   0 sidmohan   (501) staff       (20)     1811 2023-06-22 17:08:09.889730 datafog-1.2.0/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.884522 datafog-1.2.0/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.2.0/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.2.0/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.2.0/datafog/models.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.888091 datafog-1.2.0/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1811 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 17:08:09.889956 datafog-1.2.0/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)      893 2023-06-22 17:07:56.000000 datafog-1.2.0/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.889532 datafog-1.2.0/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.2.0/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.2.0/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.2.0/tests/test_models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2334 2023-06-22 17:55:46.000000 datafog-1.3.0/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.3.0/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.0/datafog/models.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.0/datafog/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.0/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.0/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.0/tests/test_models.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      893 2023-06-22 17:55:33.000000 datafog-1.3.0/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2334 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      280 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 17:55:46.000000 datafog-1.3.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `datafog-1.2.0/PKG-INFO` & `datafog-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.2.0
+Version: 1.3.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: Sid Mohan
 Author-email: sid@datafog.dev
+License: UNKNOWN
+Description: # DataFog
+        
+        DataFog (or the product formerly known as Codexify) is a Python package that simplifies and automates data anonymization tasks. With DataFog, you can quickly scan your datasets for Personal Identifiable Information (PII), swap PII with synthetic data, save and look up original and synthetic data pairs, and more.
+        
+        ## Libraries Used
+        * [faker](www.github.com/joke2k/faker) for Synthetic Data Generation
+        * Boilerplate PII detection code (swapping in with a custom solution soon)
+        
+        ## Coming Soon:
+        * product demo
+        * documentation
+        * `examples/` directory for more detailed examples and usage information
+        
+        please see www.datafog.dev for more information or contact me at sidmohan001@gmail.com
+        ## Installation
+        
+        DataFog can be installed via pip. Use the following command to install:
+        
+        ```bash
+        pip install datafog
+        ```
+        
+        ## Getting Started
+        
+        Once you've installed DataFog, you can import it into your Python scripts as follows:
+        
+        ```python
+        from datafog import DataFog
+        ```
+        
+        Now, you're ready to use DataFog to handle your PII anonymization needs. Here are some basic examples:
+        
+        **Scan a dataset for PII:**
+        
+        ```python
+        datafog = DataFog()
+        
+        # Scan a csv file for PII
+        contains_pii, pii_fields = datafog.scan("path_to_your_file.csv")
+        
+        # Print the result
+        print(f"Contains PII: {contains_pii}")
+        print(f"PII Fields: {pii_fields}")
+        ```
+        
+        **Swap PII with synthetic data:**
+        
+        ```python
+        # Define the output path
+        output_path = "path_to_output_directory/"
+        
+        # Swap PII in a csv file with synthetic data
+        datafog.swap("path_to_your_file.csv", output_path)
+        ```
+        
+        
+        ---
+        
+        
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.MD
-
-# DataFog
-
-DataFog (or the product formerly known as Codexify) is a Python package that simplifies and automates data anonymization tasks. With DataFog, you can quickly scan your datasets for Personal Identifiable Information (PII), swap PII with synthetic data, save and look up original and synthetic data pairs, and more.
-
-## Libraries Used
-* [faker](www.github.com/joke2k/faker) for Synthetic Data Generation
-* Boilerplate PII detection code (swapping in with a custom solution soon)
-
-## Coming Soon:
-* product demo
-* documentation
-* `examples/` directory for more detailed examples and usage information
-
-please see www.datafog.dev for more information or contact me at sidmohan001@gmail.com
-## Installation
-
-DataFog can be installed via pip. Use the following command to install:
-
-```bash
-pip install datafog
-```
-
-## Getting Started
-
-Once you've installed DataFog, you can import it into your Python scripts as follows:
-
-```python
-from datafog import DataFog
-```
-
-Now, you're ready to use DataFog to handle your PII anonymization needs. Here are some basic examples:
-
-**Scan a dataset for PII:**
-
-```python
-datafog = DataFog()
-
-# Scan a csv file for PII
-contains_pii, pii_fields = datafog.scan("path_to_your_file.csv")
-
-# Print the result
-print(f"Contains PII: {contains_pii}")
-print(f"PII Fields: {pii_fields}")
-```
-
-**Swap PII with synthetic data:**
-
-```python
-# Define the output path
-output_path = "path_to_output_directory/"
-
-# Swap PII in a csv file with synthetic data
-datafog.swap("path_to_your_file.csv", output_path)
-```
-
-
----
-
```

### Comparing `datafog-1.2.0/datafog/datafog.py` & `datafog-1.3.0/datafog/datafog.py`

 * *Files identical despite different names*

### Comparing `datafog-1.2.0/datafog.egg-info/PKG-INFO` & `datafog-1.3.0/datafog.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.2.0
+Version: 1.3.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: Sid Mohan
 Author-email: sid@datafog.dev
+License: UNKNOWN
+Description: # DataFog
+        
+        DataFog (or the product formerly known as Codexify) is a Python package that simplifies and automates data anonymization tasks. With DataFog, you can quickly scan your datasets for Personal Identifiable Information (PII), swap PII with synthetic data, save and look up original and synthetic data pairs, and more.
+        
+        ## Libraries Used
+        * [faker](www.github.com/joke2k/faker) for Synthetic Data Generation
+        * Boilerplate PII detection code (swapping in with a custom solution soon)
+        
+        ## Coming Soon:
+        * product demo
+        * documentation
+        * `examples/` directory for more detailed examples and usage information
+        
+        please see www.datafog.dev for more information or contact me at sidmohan001@gmail.com
+        ## Installation
+        
+        DataFog can be installed via pip. Use the following command to install:
+        
+        ```bash
+        pip install datafog
+        ```
+        
+        ## Getting Started
+        
+        Once you've installed DataFog, you can import it into your Python scripts as follows:
+        
+        ```python
+        from datafog import DataFog
+        ```
+        
+        Now, you're ready to use DataFog to handle your PII anonymization needs. Here are some basic examples:
+        
+        **Scan a dataset for PII:**
+        
+        ```python
+        datafog = DataFog()
+        
+        # Scan a csv file for PII
+        contains_pii, pii_fields = datafog.scan("path_to_your_file.csv")
+        
+        # Print the result
+        print(f"Contains PII: {contains_pii}")
+        print(f"PII Fields: {pii_fields}")
+        ```
+        
+        **Swap PII with synthetic data:**
+        
+        ```python
+        # Define the output path
+        output_path = "path_to_output_directory/"
+        
+        # Swap PII in a csv file with synthetic data
+        datafog.swap("path_to_your_file.csv", output_path)
+        ```
+        
+        
+        ---
+        
+        
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.MD
-
-# DataFog
-
-DataFog (or the product formerly known as Codexify) is a Python package that simplifies and automates data anonymization tasks. With DataFog, you can quickly scan your datasets for Personal Identifiable Information (PII), swap PII with synthetic data, save and look up original and synthetic data pairs, and more.
-
-## Libraries Used
-* [faker](www.github.com/joke2k/faker) for Synthetic Data Generation
-* Boilerplate PII detection code (swapping in with a custom solution soon)
-
-## Coming Soon:
-* product demo
-* documentation
-* `examples/` directory for more detailed examples and usage information
-
-please see www.datafog.dev for more information or contact me at sidmohan001@gmail.com
-## Installation
-
-DataFog can be installed via pip. Use the following command to install:
-
-```bash
-pip install datafog
-```
-
-## Getting Started
-
-Once you've installed DataFog, you can import it into your Python scripts as follows:
-
-```python
-from datafog import DataFog
-```
-
-Now, you're ready to use DataFog to handle your PII anonymization needs. Here are some basic examples:
-
-**Scan a dataset for PII:**
-
-```python
-datafog = DataFog()
-
-# Scan a csv file for PII
-contains_pii, pii_fields = datafog.scan("path_to_your_file.csv")
-
-# Print the result
-print(f"Contains PII: {contains_pii}")
-print(f"PII Fields: {pii_fields}")
-```
-
-**Swap PII with synthetic data:**
-
-```python
-# Define the output path
-output_path = "path_to_output_directory/"
-
-# Swap PII in a csv file with synthetic data
-datafog.swap("path_to_your_file.csv", output_path)
-```
-
-
----
-
```

### Comparing `datafog-1.2.0/setup.py` & `datafog-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Read README for the long description
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='datafog',
-    version='1.2.0',  # versioning of your package
+    version='1.3.0',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     install_requires=['faker', 'pandas','sqlalchemy','sqlalchemy.orm','werkzeug','typing','hashlib'],  # a list of other Python packages required by this package
     classifiers=[
```

### Comparing `datafog-1.2.0/tests/test_datafog.py` & `datafog-1.3.0/tests/test_datafog.py`

 * *Files identical despite different names*

