# Comparing `tmp/ppioner-0.0.3.tar.gz` & `tmp/ppioner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppioner-0.0.3.tar", last modified: Thu Jun 22 12:24:25 2023, max compression
+gzip compressed data, was "ppioner-0.0.4.tar", last modified: Thu Jun 22 12:30:43 2023, max compression
```

## Comparing `ppioner-0.0.3.tar` & `ppioner-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.621598 ppioner-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:31:35.000000 ppioner-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1322 2023-06-22 12:24:25.620598 ppioner-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-06-22 09:12:07.000000 ppioner-0.0.3/README.md
--rw-rw-rw-   0        0        0      973 2023-06-22 12:24:17.000000 ppioner-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 12:24:25.621598 ppioner-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.579598 ppioner-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.585601 ppioner-0.0.3/src/pioner/
--rw-rw-rw-   0        0        0       17 2023-06-22 07:37:28.000000 ppioner-0.0.3/src/pioner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.586600 ppioner-0.0.3/src/pioner/assets/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.3/src/pioner/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.601599 ppioner-0.0.3/src/pioner/back/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.3/src/pioner/back/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-06-22 07:25:36.000000 ppioner-0.0.3/src/pioner/back/ai_device.py
--rw-rw-rw-   0        0        0     4186 2023-06-22 07:25:36.000000 ppioner-0.0.3/src/pioner/back/ao_data_generators.py
--rw-rw-rw-   0        0        0     2845 2023-06-22 07:25:36.000000 ppioner-0.0.3/src/pioner/back/ao_device.py
--rw-rw-rw-   0        0        0     3416 2023-06-22 07:25:36.000000 ppioner-0.0.3/src/pioner/back/daq_device.py
--rw-rw-rw-   0        0        0     3031 2023-06-22 07:41:21.000000 ppioner-0.0.3/src/pioner/back/debug.py
--rw-rw-rw-   0        0        0    10394 2023-06-22 07:41:46.000000 ppioner-0.0.3/src/pioner/back/experiment_manager.py
--rw-rw-rw-   0        0        0     9782 2023-06-22 07:42:19.000000 ppioner-0.0.3/src/pioner/back/fastheat.py
--rw-rw-rw-   0        0        0     2395 2023-06-22 07:42:20.000000 ppioner-0.0.3/src/pioner/back/iso_mode.py
--rw-rw-rw-   0        0        0     6830 2023-06-22 07:42:20.000000 ppioner-0.0.3/src/pioner/back/nanocontrol_tango.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.610597 ppioner-0.0.3/src/pioner/front/
--rw-rw-rw-   0        0        0    34303 2023-06-22 07:25:36.000000 ppioner-0.0.3/src/pioner/front/SetProg_widget.py
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.3/src/pioner/front/__init__.py
--rw-rw-rw-   0        0        0    17651 2023-06-22 07:49:40.000000 ppioner-0.0.3/src/pioner/front/calibWindow.py
--rw-rw-rw-   0        0        0     5639 2023-06-22 07:49:54.000000 ppioner-0.0.3/src/pioner/front/configWindow.py
--rw-rw-rw-   0        0        0    15347 2023-06-22 07:49:24.000000 ppioner-0.0.3/src/pioner/front/mainWindow.py
--rw-rw-rw-   0        0        0    28411 2023-06-22 09:13:29.000000 ppioner-0.0.3/src/pioner/front/mainWindowUi.py
--rw-rw-rw-   0        0        0     1058 2023-04-17 10:43:41.000000 ppioner-0.0.3/src/pioner/front/messageWindows.py
--rw-rw-rw-   0        0        0    36341 2023-06-22 07:51:08.000000 ppioner-0.0.3/src/pioner/front/procFastHeatWidget.py
--rw-rw-rw-   0        0        0    16086 2023-06-22 07:51:35.000000 ppioner-0.0.3/src/pioner/front/resultsDataWidget.py
--rw-rw-rw-   0        0        0      940 2023-04-17 10:43:41.000000 ppioner-0.0.3/src/pioner/front/virtualDevice.py
--rw-rw-rw-   0        0        0      325 2023-06-22 09:20:13.000000 ppioner-0.0.3/src/pioner/runUI.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.614597 ppioner-0.0.3/src/pioner/shared/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.3/src/pioner/shared/__init__.py
--rw-rw-rw-   0        0        0     9194 2023-06-22 12:23:54.000000 ppioner-0.0.3/src/pioner/shared/calibration.py
--rw-rw-rw-   0        0        0     3501 2023-06-22 07:25:36.000000 ppioner-0.0.3/src/pioner/shared/constants.py
--rw-rw-rw-   0        0        0    14047 2023-06-22 12:15:50.000000 ppioner-0.0.3/src/pioner/shared/settings.py
--rw-rw-rw-   0        0        0     2394 2023-06-22 12:15:47.000000 ppioner-0.0.3/src/pioner/shared/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:24:25.619597 ppioner-0.0.3/src/ppioner.egg-info/
--rw-rw-rw-   0        0        0     1322 2023-06-22 12:24:25.000000 ppioner-0.0.3/src/ppioner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1079 2023-06-22 12:24:25.000000 ppioner-0.0.3/src/ppioner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:24:25.000000 ppioner-0.0.3/src/ppioner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      248 2023-06-22 12:24:25.000000 ppioner-0.0.3/src/ppioner.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 12:24:25.000000 ppioner-0.0.3/src/ppioner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.964409 ppioner-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:31:35.000000 ppioner-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1297 2023-06-22 12:30:43.964409 ppioner-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-06-22 09:12:07.000000 ppioner-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1008 2023-06-22 12:30:34.000000 ppioner-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:30:43.964409 ppioner-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.930408 ppioner-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.934410 ppioner-0.0.4/src/pioner/
+-rw-rw-rw-   0        0        0       17 2023-06-22 07:37:28.000000 ppioner-0.0.4/src/pioner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.935409 ppioner-0.0.4/src/pioner/assets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.4/src/pioner/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.946409 ppioner-0.0.4/src/pioner/back/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.4/src/pioner/back/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-06-22 07:25:36.000000 ppioner-0.0.4/src/pioner/back/ai_device.py
+-rw-rw-rw-   0        0        0     4186 2023-06-22 07:25:36.000000 ppioner-0.0.4/src/pioner/back/ao_data_generators.py
+-rw-rw-rw-   0        0        0     2845 2023-06-22 07:25:36.000000 ppioner-0.0.4/src/pioner/back/ao_device.py
+-rw-rw-rw-   0        0        0     3416 2023-06-22 07:25:36.000000 ppioner-0.0.4/src/pioner/back/daq_device.py
+-rw-rw-rw-   0        0        0     3031 2023-06-22 07:41:21.000000 ppioner-0.0.4/src/pioner/back/debug.py
+-rw-rw-rw-   0        0        0    10394 2023-06-22 07:41:46.000000 ppioner-0.0.4/src/pioner/back/experiment_manager.py
+-rw-rw-rw-   0        0        0     9782 2023-06-22 07:42:19.000000 ppioner-0.0.4/src/pioner/back/fastheat.py
+-rw-rw-rw-   0        0        0     2395 2023-06-22 07:42:20.000000 ppioner-0.0.4/src/pioner/back/iso_mode.py
+-rw-rw-rw-   0        0        0     6830 2023-06-22 07:42:20.000000 ppioner-0.0.4/src/pioner/back/nanocontrol_tango.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.954409 ppioner-0.0.4/src/pioner/front/
+-rw-rw-rw-   0        0        0    34303 2023-06-22 07:25:36.000000 ppioner-0.0.4/src/pioner/front/SetProg_widget.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.4/src/pioner/front/__init__.py
+-rw-rw-rw-   0        0        0    17651 2023-06-22 07:49:40.000000 ppioner-0.0.4/src/pioner/front/calibWindow.py
+-rw-rw-rw-   0        0        0     5639 2023-06-22 07:49:54.000000 ppioner-0.0.4/src/pioner/front/configWindow.py
+-rw-rw-rw-   0        0        0    15347 2023-06-22 07:49:24.000000 ppioner-0.0.4/src/pioner/front/mainWindow.py
+-rw-rw-rw-   0        0        0    28411 2023-06-22 09:13:29.000000 ppioner-0.0.4/src/pioner/front/mainWindowUi.py
+-rw-rw-rw-   0        0        0     1058 2023-04-17 10:43:41.000000 ppioner-0.0.4/src/pioner/front/messageWindows.py
+-rw-rw-rw-   0        0        0    36341 2023-06-22 07:51:08.000000 ppioner-0.0.4/src/pioner/front/procFastHeatWidget.py
+-rw-rw-rw-   0        0        0    16086 2023-06-22 07:51:35.000000 ppioner-0.0.4/src/pioner/front/resultsDataWidget.py
+-rw-rw-rw-   0        0        0      940 2023-04-17 10:43:41.000000 ppioner-0.0.4/src/pioner/front/virtualDevice.py
+-rw-rw-rw-   0        0        0      325 2023-06-22 09:20:13.000000 ppioner-0.0.4/src/pioner/runUI.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.958409 ppioner-0.0.4/src/pioner/shared/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.4/src/pioner/shared/__init__.py
+-rw-rw-rw-   0        0        0     9194 2023-06-22 12:23:54.000000 ppioner-0.0.4/src/pioner/shared/calibration.py
+-rw-rw-rw-   0        0        0     3501 2023-06-22 07:25:36.000000 ppioner-0.0.4/src/pioner/shared/constants.py
+-rw-rw-rw-   0        0        0    14047 2023-06-22 12:15:50.000000 ppioner-0.0.4/src/pioner/shared/settings.py
+-rw-rw-rw-   0        0        0     2394 2023-06-22 12:15:47.000000 ppioner-0.0.4/src/pioner/shared/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:43.963410 ppioner-0.0.4/src/ppioner.egg-info/
+-rw-rw-rw-   0        0        0     1297 2023-06-22 12:30:43.000000 ppioner-0.0.4/src/ppioner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2023-06-22 12:30:43.000000 ppioner-0.0.4/src/ppioner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:30:43.000000 ppioner-0.0.4/src/ppioner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-22 12:30:43.000000 ppioner-0.0.4/src/ppioner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      229 2023-06-22 12:30:43.000000 ppioner-0.0.4/src/ppioner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 12:30:43.000000 ppioner-0.0.4/src/ppioner.egg-info/top_level.txt
```

### Comparing `ppioner-0.0.3/PKG-INFO` & `ppioner-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ppioner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic software to operate PIONER device (former Nanocal)
 Author-email: awesome author <awesome@author.edu>
 License: MIT
 Keywords: nanocalorimetry,DAQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: server
 Provides-Extra: gui
-Provides-Extra: dynamic
 License-File: LICENSE
 
 # Nanocal
 
 
 ## 1. Install MCC Universal Library for Linux (uldaq)
```

### Comparing `ppioner-0.0.3/README.md` & `ppioner-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/pyproject.toml` & `ppioner-0.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0", 
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ppioner"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "awesome author", email = "awesome@author.edu"},
 ]
 description = "Basic software to operate PIONER device (former Nanocal)"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["nanocalorimetry", "DAQ"]
@@ -33,9 +33,9 @@
     'importlib-metadata; python_version<"3.8"',
 ]
 
 [project.optional-dependencies]
 server = ["uldaq==1.2.3",]
 gui = ["silx==1.0.0", "pyqt5==5.15.6",]
 
-
-dynamic = ["version"]
+[project.scripts]
+pionerUI = "pioner.runUI:pioner_run_ui"
```

### Comparing `ppioner-0.0.3/src/pioner/back/ai_device.py` & `ppioner-0.0.4/src/pioner/back/ai_device.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/ao_data_generators.py` & `ppioner-0.0.4/src/pioner/back/ao_data_generators.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/ao_device.py` & `ppioner-0.0.4/src/pioner/back/ao_device.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/daq_device.py` & `ppioner-0.0.4/src/pioner/back/daq_device.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/debug.py` & `ppioner-0.0.4/src/pioner/back/debug.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/experiment_manager.py` & `ppioner-0.0.4/src/pioner/back/experiment_manager.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/fastheat.py` & `ppioner-0.0.4/src/pioner/back/fastheat.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/iso_mode.py` & `ppioner-0.0.4/src/pioner/back/iso_mode.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/back/nanocontrol_tango.py` & `ppioner-0.0.4/src/pioner/back/nanocontrol_tango.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/SetProg_widget.py` & `ppioner-0.0.4/src/pioner/front/SetProg_widget.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/calibWindow.py` & `ppioner-0.0.4/src/pioner/front/calibWindow.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/configWindow.py` & `ppioner-0.0.4/src/pioner/front/configWindow.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/mainWindow.py` & `ppioner-0.0.4/src/pioner/front/mainWindow.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/mainWindowUi.py` & `ppioner-0.0.4/src/pioner/front/mainWindowUi.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/messageWindows.py` & `ppioner-0.0.4/src/pioner/front/messageWindows.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/procFastHeatWidget.py` & `ppioner-0.0.4/src/pioner/front/procFastHeatWidget.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/resultsDataWidget.py` & `ppioner-0.0.4/src/pioner/front/resultsDataWidget.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/front/virtualDevice.py` & `ppioner-0.0.4/src/pioner/front/virtualDevice.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/shared/calibration.py` & `ppioner-0.0.4/src/pioner/shared/calibration.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/shared/constants.py` & `ppioner-0.0.4/src/pioner/shared/constants.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/shared/settings.py` & `ppioner-0.0.4/src/pioner/shared/settings.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/pioner/shared/utils.py` & `ppioner-0.0.4/src/pioner/shared/utils.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.3/src/ppioner.egg-info/PKG-INFO` & `ppioner-0.0.4/src/ppioner.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ppioner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic software to operate PIONER device (former Nanocal)
 Author-email: awesome author <awesome@author.edu>
 License: MIT
 Keywords: nanocalorimetry,DAQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: server
 Provides-Extra: gui
-Provides-Extra: dynamic
 License-File: LICENSE
 
 # Nanocal
 
 
 ## 1. Install MCC Universal Library for Linux (uldaq)
```

### Comparing `ppioner-0.0.3/src/ppioner.egg-info/SOURCES.txt` & `ppioner-0.0.4/src/ppioner.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 src/pioner/shared/calibration.py
 src/pioner/shared/constants.py
 src/pioner/shared/settings.py
 src/pioner/shared/utils.py
 src/ppioner.egg-info/PKG-INFO
 src/ppioner.egg-info/SOURCES.txt
 src/ppioner.egg-info/dependency_links.txt
+src/ppioner.egg-info/entry_points.txt
 src/ppioner.egg-info/requires.txt
 src/ppioner.egg-info/top_level.txt
```

