# Comparing `tmp/autonicer-1.2.5.tar.gz` & `tmp/autonicer-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonicer-1.2.5.tar", max compression
+gzip compressed data, was "autonicer-1.2.6.tar", last modified: Thu Jun 22 04:52:28 2023, max compression
```

## Comparing `autonicer-1.2.5.tar` & `autonicer-1.2.6.tar`

### file list

```diff
@@ -1,9 +1,25 @@
--rw-r--r--   0        0        0    11346 2022-12-01 00:31:33.500519 autonicer-1.2.5/LICENSE
--rw-r--r--   0        0        0     4445 2023-01-11 22:11:53.995829 autonicer-1.2.5/README.md
--rw-r--r--   0        0        0     1808 2023-01-08 05:50:13.454342 autonicer-1.2.5/autonicer/__init__.py
--rw-r--r--   0        0        0       53 2022-12-01 00:31:33.500519 autonicer-1.2.5/autonicer/__main__.py
--rw-r--r--   0        0        0    13499 2023-01-11 22:11:53.995829 autonicer-1.2.5/autonicer/autonicer.py
--rw-r--r--   0        0        0     7321 2023-01-11 02:18:15.519581 autonicer-1.2.5/autonicer/reprocess.py
--rw-r--r--   0        0        0      725 2023-02-16 15:46:05.035746 autonicer-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     5492 1970-01-01 00:00:00.000000 autonicer-1.2.5/setup.py
--rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 autonicer-1.2.5/PKG-INFO
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-22 04:52:28.767391 autonicer-1.2.6/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      325 2023-06-22 04:18:06.000000 autonicer-1.2.6/.gitignore
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5446 2023-03-29 02:14:17.000000 autonicer-1.2.6/CHANGELOG.md
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6146 2023-05-02 20:47:11.000000 autonicer-1.2.6/Dockerfile
+-rw-rw-r--   0 nick      (1000) nick      (1000)    11346 2021-11-21 18:21:51.000000 autonicer-1.2.6/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    17894 2023-06-22 04:52:28.767391 autonicer-1.2.6/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4572 2023-03-29 02:14:17.000000 autonicer-1.2.6/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-22 04:52:28.763391 autonicer-1.2.6/autonicer/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1808 2023-03-29 02:14:17.000000 autonicer-1.2.6/autonicer/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       53 2022-05-08 03:07:39.000000 autonicer-1.2.6/autonicer/__main__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13533 2023-06-22 04:19:41.000000 autonicer-1.2.6/autonicer/autonicer.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7321 2023-04-10 21:25:21.000000 autonicer-1.2.6/autonicer/reprocess.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-22 04:52:28.763391 autonicer-1.2.6/autonicer.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    17894 2023-06-22 04:52:28.000000 autonicer-1.2.6/autonicer.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      416 2023-06-22 04:52:28.000000 autonicer-1.2.6/autonicer.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-22 04:52:28.000000 autonicer-1.2.6/autonicer.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       44 2023-06-22 04:52:28.000000 autonicer-1.2.6/autonicer.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      210 2023-06-22 04:52:28.000000 autonicer-1.2.6/autonicer.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       10 2023-06-22 04:52:28.000000 autonicer-1.2.6/autonicer.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      925 2023-06-22 04:48:19.000000 autonicer-1.2.6/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)      752 2023-06-22 04:50:25.000000 autonicer-1.2.6/requirements.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-06-22 04:52:28.767391 autonicer-1.2.6/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-22 04:52:28.767391 autonicer-1.2.6/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-05-08 03:07:39.000000 autonicer-1.2.6/tests/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     8612 2023-03-29 02:14:17.000000 autonicer-1.2.6/tests/test_autonicer.py
```

### Comparing `autonicer-1.2.5/LICENSE` & `autonicer-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autonicer-1.2.5/README.md` & `autonicer-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [![PyPI](https://img.shields.io/pypi/v/autonicer.svg)](https://pypi.org/project/autonicer/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/autonicer.svg?label=PyPI%20downloads)](https://pypi.org/project/autonicer/)
+
 # autoNICER
 A piece of software that allows for the automated retrieval, and default data reduction of NICER data. This software was developed to automate the retrieval of NICER data and perform standardized data reduction on the retrieved NICER data. 
 This project unaffiliated with the NICER team, NASA, the Goddard Space Flight Center (GSFC), and HEASARC. Thus, under no circumstances should anyone consider this project endorsed or recommended by the afformentioned agencies and organizations.
 
 ## Contributing
 Anyone considering contribiting to this project is encouraged to do so.
 Constributing can be something as small as submitting issues you have found or requesting enhancements. Your feedback is incredibly valuable for improving the project.
```

### Comparing `autonicer-1.2.5/autonicer/__init__.py` & `autonicer-1.2.6/autonicer/__init__.py`

 * *Files identical despite different names*

### Comparing `autonicer-1.2.5/autonicer/autonicer.py` & `autonicer-1.2.6/autonicer/autonicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     def call_nicer(self):
         """
         Querys the nicermastr catalog for all observations of the specified source(self.obj)
         """
         heasarc = Heasarc()
         try:
             warnings.simplefilter("ignore", category=AstropyWarning)
+            Heasarc.clear_cache()
             xti = heasarc.query_object(
                 self.obj, mission="nicermastr"
             )  # calls NICER master catalogue for an input object
         except exceptions.InvalidQueryError:
             print(colored(f"UNABLE TO RESOLVE {self.obj} in HEASARC!", "red"))
             print(colored(f"Exiting ...", "red"))
             exit()
```

### Comparing `autonicer-1.2.5/autonicer/reprocess.py` & `autonicer-1.2.6/autonicer/reprocess.py`

 * *Files identical despite different names*

