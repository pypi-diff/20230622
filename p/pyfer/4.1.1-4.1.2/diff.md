# Comparing `tmp/pyfer-4.1.1.tar.gz` & `tmp/pyfer-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfer-4.1.1.tar", last modified: Tue Jun 20 16:19:31 2023, max compression
+gzip compressed data, was "pyfer-4.1.2.tar", last modified: Thu Jun 22 15:30:27 2023, max compression
```

## Comparing `pyfer-4.1.1.tar` & `pyfer-4.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:19:31.642626 pyfer-4.1.1/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1065 2023-04-03 07:33:30.000000 pyfer-4.1.1/LICENSE.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)     1944 2023-06-20 16:19:31.641928 pyfer-4.1.1/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)     1292 2023-06-20 16:06:14.000000 pyfer-4.1.1/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:19:31.635771 pyfer-4.1.1/pyfer/
--rw-r--r--   0 lucbatty   (501) staff       (20)       46 2023-04-03 07:33:30.000000 pyfer-4.1.1/pyfer/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    10451 2023-06-20 09:28:21.000000 pyfer-4.1.1/pyfer/pyfer.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:19:31.641065 pyfer-4.1.1/pyfer.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1944 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      194 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      226 2023-04-03 07:33:30.000000 pyfer-4.1.1/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 16:19:31.642868 pyfer-4.1.1/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      852 2023-06-20 16:11:32.000000 pyfer-4.1.1/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 15:30:27.384426 pyfer-4.1.2/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1065 2023-04-03 07:33:30.000000 pyfer-4.1.2/LICENSE.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2025 2023-06-22 15:30:27.383784 pyfer-4.1.2/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1623 2023-06-22 15:28:33.000000 pyfer-4.1.2/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 15:30:27.379191 pyfer-4.1.2/pyfer/
+-rw-r--r--   0 lucbatty   (501) staff       (20)       46 2023-04-03 07:33:30.000000 pyfer-4.1.2/pyfer/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    10451 2023-06-22 10:56:16.000000 pyfer-4.1.2/pyfer/pyfer.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 15:30:27.382676 pyfer-4.1.2/pyfer.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2025 2023-06-22 15:30:27.000000 pyfer-4.1.2/pyfer.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      194 2023-06-22 15:30:27.000000 pyfer-4.1.2/pyfer.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-22 15:30:27.000000 pyfer-4.1.2/pyfer.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-22 15:30:27.000000 pyfer-4.1.2/pyfer.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      226 2023-04-03 07:33:30.000000 pyfer-4.1.2/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-22 15:30:27.384685 pyfer-4.1.2/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      607 2023-06-22 15:05:14.000000 pyfer-4.1.2/setup.py
```

### Comparing `pyfer-4.1.1/LICENSE.txt` & `pyfer-4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfer-4.1.1/PKG-INFO` & `pyfer-4.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: pyfer
-Version: 4.1.1
+Version: 4.1.2
 Summary: Simple String Encryption Toolkit
 Home-page: https://github.com/celerygemini/pyfer
 Author: celerygemini
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![pyfer_cover](aux/rm_cover.jpg)
 
 -----------------
 
@@ -40,29 +35,32 @@
 
 ## 🛠️ Setup 
 
 Install it from **PyPI** by running `pip install pyfer`.
 
 ### Dependencies 
 
-The only dependency is [NumPy](https://numpy.org)
+The only dependency is [NumPy](https://numpy.org).
 
 ## 🚀 Execution
 
-### Quickstart
+### App
 
-```
-import pyfer
+If running in a virtual environment using `pyenv`/`virtualenv`, ensure the Python version is configured for `tkinter` by following the instructions [here](https://github.com/celerygemini/resources/blob/main/pyenv_tkinter.md).
 
-k = pyfer.generate_key(45)
-m = "Hello_world!"
-pm = pyfer.Machine(k)
+To run the app, simply open a terminal window to the project folder and run:
+```
+python app.py
+```
 
-pm.scramble(m)
+### Command Line
 
+Alternatively, Pyfer can be run from the command line:
+```
+python main.py <key> <input_string>
 ```
 
 For more information, have a look at the demo [here](https://github.com/elbydata/pyfer/blob/master/demos/demo.ipynb)!
 
 ## 📝 Documentation
 
 Documentation is currently available in the form of docstrings.
```

### Comparing `pyfer-4.1.1/pyfer/pyfer.py` & `pyfer-4.1.2/pyfer/pyfer.py`

 * *Files identical despite different names*

### Comparing `pyfer-4.1.1/pyfer.egg-info/PKG-INFO` & `pyfer-4.1.2/pyfer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: pyfer
-Version: 4.1.1
+Version: 4.1.2
 Summary: Simple String Encryption Toolkit
 Home-page: https://github.com/celerygemini/pyfer
 Author: celerygemini
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![pyfer_cover](aux/rm_cover.jpg)
 
 -----------------
 
@@ -40,29 +35,32 @@
 
 ## 🛠️ Setup 
 
 Install it from **PyPI** by running `pip install pyfer`.
 
 ### Dependencies 
 
-The only dependency is [NumPy](https://numpy.org)
+The only dependency is [NumPy](https://numpy.org).
 
 ## 🚀 Execution
 
-### Quickstart
+### App
 
-```
-import pyfer
+If running in a virtual environment using `pyenv`/`virtualenv`, ensure the Python version is configured for `tkinter` by following the instructions [here](https://github.com/celerygemini/resources/blob/main/pyenv_tkinter.md).
 
-k = pyfer.generate_key(45)
-m = "Hello_world!"
-pm = pyfer.Machine(k)
+To run the app, simply open a terminal window to the project folder and run:
+```
+python app.py
+```
 
-pm.scramble(m)
+### Command Line
 
+Alternatively, Pyfer can be run from the command line:
+```
+python main.py <key> <input_string>
 ```
 
 For more information, have a look at the demo [here](https://github.com/elbydata/pyfer/blob/master/demos/demo.ipynb)!
 
 ## 📝 Documentation
 
 Documentation is currently available in the form of docstrings.
```

### Comparing `pyfer-4.1.1/setup.py` & `pyfer-4.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfer",
-    version="4.1.1",
+    version="4.1.2",
     author="celerygemini",
     description="Simple String Encryption Toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/celerygemini/pyfer",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.11",
 )
```

