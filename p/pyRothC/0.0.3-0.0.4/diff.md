# Comparing `tmp/pyRothC-0.0.3.tar.gz` & `tmp/pyrothc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRothC-0.0.3.tar", last modified: Wed May 31 20:26:20 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyRothC-0.0.3.tar` & `pyrothc-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,20 @@
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.857877 pyRothC-0.0.3/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)     1834 2023-05-31 20:17:09.000000 pyRothC-0.0.3/.gitignore
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)     7048 2022-10-29 10:17:12.000000 pyRothC-0.0.3/LICENSE
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    12953 2023-05-31 20:26:20.856849 pyRothC-0.0.3/PKG-INFO
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)     3816 2023-05-31 20:17:09.000000 pyRothC-0.0.3/README.md
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.843214 pyRothC-0.0.3/notebooks/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    73445 2023-03-05 20:21:46.000000 pyRothC-0.0.3/notebooks/pyRothC.ipynb
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.846913 pyRothC-0.0.3/plots/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    16308 2023-03-04 11:17:28.000000 pyRothC-0.0.3/plots/Logo.svg
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    50344 2023-03-02 11:58:47.000000 pyRothC-0.0.3/plots/moisture_factor.png
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    45995 2023-03-02 11:59:35.000000 pyRothC-0.0.3/plots/soil_clay_factor.png
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    68569 2023-03-02 11:58:17.000000 pyRothC-0.0.3/plots/temp_factor.png
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.848395 pyRothC-0.0.3/pyRothC/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    10905 2023-05-31 20:17:09.000000 pyRothC-0.0.3/pyRothC/RothC.py
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)        0 2023-03-04 12:14:32.000000 pyRothC-0.0.3/pyRothC/__init__.py
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.851878 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)    12953 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/PKG-INFO
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)      483 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/SOURCES.txt
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)        1 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/dependency_links.txt
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)       56 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/requires.txt
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)        1 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/top_level.txt
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)     1356 2023-05-31 20:24:07.000000 pyRothC-0.0.3/pyproject.toml
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)       38 2023-05-31 20:26:20.858074 pyRothC-0.0.3/setup.cfg
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)       38 2023-03-04 10:37:19.000000 pyRothC-0.0.3/setup.py
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.854342 pyRothC-0.0.3/tests/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/__init__.py
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)      261 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/conftest.py
-drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.855374 pyRothC-0.0.3/tests/data/
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)     2269 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/data/2years_results.csv
--rw-r--r--   0 mikhailgasanov   (501) staff       (20)      919 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/test_rothc.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyrothc-0.0.4/.DS_Store
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyrothc-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyrothc-0.0.4/examples/.DS_Store
+-rw-r--r--   0        0        0    73445 2020-02-02 00:00:00.000000 pyrothc-0.0.4/notebooks/pyRothC.ipynb
+-rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 pyrothc-0.0.4/plots/Logo.svg
+-rw-r--r--   0        0        0    50344 2020-02-02 00:00:00.000000 pyrothc-0.0.4/plots/moisture_factor.png
+-rw-r--r--   0        0        0    45995 2020-02-02 00:00:00.000000 pyrothc-0.0.4/plots/soil_clay_factor.png
+-rw-r--r--   0        0        0    68569 2020-02-02 00:00:00.000000 pyrothc-0.0.4/plots/temp_factor.png
+-rw-r--r--   0        0        0    10910 2020-02-02 00:00:00.000000 pyrothc-0.0.4/pyRothC/RothC.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrothc-0.0.4/pyRothC/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrothc-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyrothc-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyrothc-0.0.4/tests/test_rothc.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrothc-0.0.4/tests/data/2years_results.csv
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 pyrothc-0.0.4/tests/data/9years_results.csv
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 pyrothc-0.0.4/.gitignore
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 pyrothc-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 pyrothc-0.0.4/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 pyrothc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    13068 2020-02-02 00:00:00.000000 pyrothc-0.0.4/PKG-INFO
```

### Comparing `pyRothC-0.0.3/.gitignore` & `pyrothc-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/LICENSE` & `pyrothc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/PKG-INFO` & `pyrothc-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: pyRothC
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python version of The Rothamsted carbon model (RothC) 26.3. RothC is a model for the turnover of organic carbon in non-waterlogged topsoil that allows for the effects of soil type, temperature, soil moisture and plant cover on the turnover process.
+Project-URL: Documentation, https://mishagrol.github.io
+Project-URL: Source code, https://github.com/mishagrol/pyRothC
 Author-email: Misha Grol <grol81@mail.ru>
 Maintainer: misha grol
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -121,31 +123,32 @@
             limitation any person's Copyright and Related Rights in the Work.
             Further, Affirmer disclaims responsibility for obtaining any necessary
             consents, permissions or other rights required for any use of the
             Work.
          d. Affirmer understands and acknowledges that Creative Commons is not a
             party to this document and has no duty or obligation with respect to
             this CC0 or use of the Work.
-        
-Project-URL: Documentation, https://mishagrol.github.io
-Project-URL: Source code, https://github.com/mishagrol/pyRothC
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: pandas>=1.3.4
+Requires-Dist: scipy>=1.7.3
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == 'test'
+Description-Content-Type: text/markdown
 
 ## pyRothC
 <p align="center">
 <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/mishagrol/pyRothC?style=social">
 
 <a href="https://github.com/mishagrol/pyRothC/issues" target="_blank">
     <img src="https://img.shields.io/github/issues/mishagrol/pyRothC" alt="Issues">
@@ -295,8 +298,8 @@
 $$
 ## Optional Dependencies
 
 Matplotlib
 
 ## License
 
-This project is licensed under the terms of the CC0 1.0 Universal license.
+This project is licensed under the terms of the CC0 1.0 Universal license.
```

### Comparing `pyRothC-0.0.3/README.md` & `pyrothc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/notebooks/pyRothC.ipynb` & `pyrothc-0.0.4/notebooks/pyRothC.ipynb`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/plots/Logo.svg` & `pyrothc-0.0.4/plots/Logo.svg`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/plots/moisture_factor.png` & `pyrothc-0.0.4/plots/moisture_factor.png`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/plots/soil_clay_factor.png` & `pyrothc-0.0.4/plots/soil_clay_factor.png`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/plots/temp_factor.png` & `pyrothc-0.0.4/plots/temp_factor.png`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/pyRothC/RothC.py` & `pyrothc-0.0.4/pyRothC/RothC.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             solver (str, optional): Solver - Not implemented yet. Defaults to "euler".
 
         Raises:
             ValueError: _description_
             ValueError: _description_
         """
         self.years = years
-        self.t = np.arange(1 / 12, years, step=1 / 12)
+        self.t = np.linspace(1 / 12, years, num=years * 12)
         self.ks_pulls = ["DPM", "RPM", "BIO", "HUM", "IOM"]
         if len(ks) != 5:
             raise ValueError("ks must be of length = 5")
         self.ks = ks
         if len(C0) != 5:
             raise ValueError("the vector with initial conditions must be of length = 5")
         self.C0 = C0
```

### Comparing `pyRothC-0.0.3/pyproject.toml` & `pyrothc-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.8.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyRothC"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python version of The Rothamsted carbon model (RothC) 26.3. RothC is a model for the turnover of organic carbon in non-waterlogged topsoil that allows for the effects of soil type, temperature, soil moisture and plant cover on the turnover process."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   { name = "Misha Grol", email = "grol81@mail.ru" }
 ]
```

### Comparing `pyRothC-0.0.3/tests/data/2years_results.csv` & `pyrothc-0.0.4/tests/data/2years_results.csv`

 * *Files identical despite different names*

### Comparing `pyRothC-0.0.3/tests/test_rothc.py` & `pyrothc-0.0.4/tests/test_rothc.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,7 +21,32 @@
         pE=1.0,
         C0=np.array([0, 0, 0, 0, inert_organic_matter])
     )
 
     dataframe = rothc.compute()
 
     assert_frame_equal(dataframe, results_2years)
+
+
+def test_compute_sequence_endpoint(results_9years):
+    """The time sequence can miss the endpoint value in some scenarios. Ensure this is sorted out
+    and all values are computed.
+    """
+    temperature = np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9, 18.0, 17.5, 13.4, 8.7, 3.9, 0.6])
+    precipitation = np.array([49, 39, 44, 41, 61, 58, 71, 58, 51, 48, 50, 58])
+    evaporation = np.array([12, 18, 35, 58, 82, 90, 97, 84, 54, 31, 14, 10])
+    inert_organic_matter = 0.049 * 69.7 ** 1.139
+
+    rothc = RothC(
+        temperature=temperature,
+        precip=precipitation,
+        evaporation=evaporation,
+        years=9,  # Test the results for 9 years, which might fail if we use a step of 1 / 12.
+        clay=48,
+        input_carbon=2.7,
+        pE=1.0,
+        C0=np.array([0, 0, 0, 0, inert_organic_matter])
+    )
+
+    dataframe = rothc.compute()
+
+    assert_frame_equal(dataframe, results_9years)
```

