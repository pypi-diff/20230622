# Comparing `tmp/fa-models-1.0.40.tar.gz` & `tmp/fa-models-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.40.tar", last modified: Tue Apr  4 08:33:27 2023, max compression
+gzip compressed data, was "fa-models-1.0.43.tar", last modified: Thu Jun 22 12:09:54 2023, max compression
```

## Comparing `fa-models-1.0.40.tar` & `fa-models-1.0.43.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 08:33:27.057471 fa-models-1.0.40/
--rw-rw-rw-   0        0        0     3289 2023-04-04 08:33:27.055941 fa-models-1.0.40/PKG-INFO
--rw-rw-rw-   0        0        0     2725 2023-03-26 19:57:42.000000 fa-models-1.0.40/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 08:33:26.972805 fa-models-1.0.40/fa_models.egg-info/
--rw-rw-rw-   0        0        0     3289 2023-04-04 08:33:26.000000 fa-models-1.0.40/fa_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-04-04 08:33:26.000000 fa-models-1.0.40/fa_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 08:33:26.000000 fa-models-1.0.40/fa_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-04 08:33:26.000000 fa-models-1.0.40/fa_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 08:33:26.000000 fa-models-1.0.40/fa_models.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 08:33:26.976800 fa-models-1.0.40/famodels/
--rw-rw-rw-   0        0        0        0 2023-03-18 09:51:48.000000 fa-models-1.0.40/famodels/__init__.py
--rw-rw-rw-   0        0        0       92 2023-03-18 09:48:40.000000 fa-models-1.0.40/famodels/direction.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:33:26.984918 fa-models-1.0.40/famodels/generators/
--rw-rw-rw-   0        0        0        0 2023-03-18 09:47:08.000000 fa-models-1.0.40/famodels/generators/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-03-26 21:17:57.000000 fa-models-1.0.40/famodels/generators/data_generator.py
--rw-rw-rw-   0        0        0    11151 2023-03-23 08:14:14.000000 fa-models-1.0.40/famodels/generators/schema_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:33:27.023588 fa-models-1.0.40/famodels/models/
--rw-rw-rw-   0        0        0        0 2023-03-18 09:14:45.000000 fa-models-1.0.40/famodels/models/__init__.py
--rw-rw-rw-   0        0        0       92 2023-01-19 12:24:54.000000 fa-models-1.0.40/famodels/models/direction.py
--rw-rw-rw-   0        0        0     1326 2023-03-21 22:15:20.000000 fa-models-1.0.40/famodels/models/order.py
--rw-rw-rw-   0        0        0       96 2023-01-19 12:25:47.000000 fa-models-1.0.40/famodels/models/order_type.py
--rw-rw-rw-   0        0        0      663 2023-04-04 07:57:41.000000 fa-models-1.0.40/famodels/models/processed_trading_signal.py
--rw-rw-rw-   0        0        0       83 2023-01-19 12:24:30.000000 fa-models-1.0.40/famodels/models/side.py
--rw-rw-rw-   0        0        0      272 2023-03-26 19:52:53.000000 fa-models-1.0.40/famodels/models/state_of_signal.py
--rw-rw-rw-   0        0        0      884 2023-01-19 12:25:20.000000 fa-models-1.0.40/famodels/models/state_of_trade.py
--rw-rw-rw-   0        0        0     1890 2023-03-18 09:33:40.000000 fa-models-1.0.40/famodels/models/trade.py
--rw-rw-rw-   0        0        0     3083 2023-03-26 21:19:21.000000 fa-models-1.0.40/famodels/models/trading_signal.py
--rw-rw-rw-   0        0        0     1342 2023-04-04 08:32:51.000000 fa-models-1.0.40/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 08:33:27.057471 fa-models-1.0.40/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-03-18 09:51:35.000000 fa-models-1.0.40/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:33:27.051433 fa-models-1.0.40/tests/
--rw-rw-rw-   0        0        0      272 2023-03-18 09:52:10.000000 fa-models-1.0.40/tests/test_data_generator.py
--rw-rw-rw-   0        0        0     1347 2023-04-04 07:50:01.000000 fa-models-1.0.40/tests/test_processed_trading_signal.py
--rw-rw-rw-   0        0        0      857 2023-03-18 09:37:22.000000 fa-models-1.0.40/tests/test_produce_schemas.py
--rw-rw-rw-   0        0        0     2338 2023-03-22 15:14:28.000000 fa-models-1.0.40/tests/test_schema_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.778478 fa-models-1.0.43/
+-rw-rw-rw-   0        0        0     3510 2023-06-22 12:09:54.776020 fa-models-1.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0     2946 2023-06-22 12:07:42.000000 fa-models-1.0.43/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.695349 fa-models-1.0.43/fa_models.egg-info/
+-rw-rw-rw-   0        0        0     3510 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.702810 fa-models-1.0.43/famodels/
+-rw-rw-rw-   0        0        0        0 2023-03-18 09:51:48.000000 fa-models-1.0.43/famodels/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-03-18 09:48:40.000000 fa-models-1.0.43/famodels/direction.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.714328 fa-models-1.0.43/famodels/generators/
+-rw-rw-rw-   0        0        0        0 2023-03-18 09:47:08.000000 fa-models-1.0.43/famodels/generators/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-03-26 21:17:57.000000 fa-models-1.0.43/famodels/generators/data_generator.py
+-rw-rw-rw-   0        0        0    11151 2023-03-23 08:14:14.000000 fa-models-1.0.43/famodels/generators/schema_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.755856 fa-models-1.0.43/famodels/models/
+-rw-rw-rw-   0        0        0        0 2023-03-18 09:14:45.000000 fa-models-1.0.43/famodels/models/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-01-19 12:24:54.000000 fa-models-1.0.43/famodels/models/direction.py
+-rw-rw-rw-   0        0        0     1374 2023-06-18 19:02:13.000000 fa-models-1.0.43/famodels/models/order.py
+-rw-rw-rw-   0        0        0       96 2023-01-19 12:25:47.000000 fa-models-1.0.43/famodels/models/order_type.py
+-rw-rw-rw-   0        0        0     1275 2023-06-18 19:01:06.000000 fa-models-1.0.43/famodels/models/processed_signal.py
+-rw-rw-rw-   0        0        0       83 2023-01-19 12:24:30.000000 fa-models-1.0.43/famodels/models/side.py
+-rw-rw-rw-   0        0        0      274 2023-06-13 12:35:17.000000 fa-models-1.0.43/famodels/models/state_of_signal.py
+-rw-rw-rw-   0        0        0      884 2023-01-19 12:25:20.000000 fa-models-1.0.43/famodels/models/state_of_trade.py
+-rw-rw-rw-   0        0        0     1890 2023-03-18 09:33:40.000000 fa-models-1.0.43/famodels/models/trade.py
+-rw-rw-rw-   0        0        0     3293 2023-06-18 19:01:29.000000 fa-models-1.0.43/famodels/models/trading_signal.py
+-rw-rw-rw-   0        0        0     1854 2023-06-18 19:00:18.000000 fa-models-1.0.43/famodels/models/virtual_order.py
+-rw-rw-rw-   0        0        0     1342 2023-06-22 12:09:22.000000 fa-models-1.0.43/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:09:54.779509 fa-models-1.0.43/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-03-18 09:51:35.000000 fa-models-1.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.771441 fa-models-1.0.43/tests/
+-rw-rw-rw-   0        0        0      272 2023-03-18 09:52:10.000000 fa-models-1.0.43/tests/test_data_generator.py
+-rw-rw-rw-   0        0        0     1427 2023-06-13 13:04:30.000000 fa-models-1.0.43/tests/test_processed_trading_signal.py
+-rw-rw-rw-   0        0        0      857 2023-03-18 09:37:22.000000 fa-models-1.0.43/tests/test_produce_schemas.py
+-rw-rw-rw-   0        0        0     2338 2023-03-22 15:14:28.000000 fa-models-1.0.43/tests/test_schema_generator.py
```

### Comparing `fa-models-1.0.40/PKG-INFO` & `fa-models-1.0.43/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.40
+Version: 1.0.43
 Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -34,52 +34,98 @@
 ### Installation as Consuming Developer
 
 Simply run: `pip install fa-models`
 
 Import in modules without the dash (e.g.): `from famodels.signal import Signal`
 
 ### Setup as Contributor
-Create the virtul environment: `py -m venv .venv`
-Start the Environment: `./.venv/Scripts/activate`. Use `deactivate`to stop it.
-Update the PIP: `py -m pip install --upgrade pip`
-
-All the required libraries must be listed in requirements.txt and installed by  `py -m pip install -r .\requirements.txt`
+Create the virtul environment: 
+```
+py -m venv .venv
+```
+Start the Environment: 
+```
+./.venv/Scripts/activate
+```
+ (or allow VS Code to start it). Use `deactivate`to stop it.
+
+All the required libraries must be listed in requirements.txt and installed by  
+```
+python -m pip install -r .\requirements.txt
+```
+For Dev use 
+```
+python -m pip install -r .\requirements-dev.txt
+```
 
 To cleanup the environment run:
-`pip3 freeze > to-uninstall.txt` and then
-`pip3 uninstall -y -r to-uninstall.txt`
-
-or `pip3 install pip-autoremove`
+```
+pip3 freeze > to-uninstall.txt
+```
+ and then
+```
+pip3 uninstall -y -r to-uninstall.txt
+```
+
+or 
+```
+pip3 install pip-autoremove
+```
 
 ### Build Library
 Prerequisite: make sure that you give your Operating System user the right to modify files in the python directory. The directory where pyhton is installed.
 Use `python setup.py bdist_wheel` to create the dist, build and .eggs folder.
 
 ## Reference from a different project
 In order to use your own version of the project - to maybe contribute to the library - simply clone the code from github into new directory. Then add the path of that new directory to the requirements.txt file of your project. Then change in fa-models whatever you recommend to improve. Don't forget the Open-Closed Principle: extend only (unless it requires a breaking change)
 
 
 ### Releasing a new version
 
 Delete any old files in the /dist and build folder of your local environment.
-Update your pip: `python -m pip install --upgrade pip`
-
-Install the tools build, twine and bumpver: `python -m pip install build twine bumpver`
-Upgrade the setuptools: `pip install --upgrade setuptools`
-
-Bump the version in pyproject.toml: `bumpver update --patch`
+Update your pip: 
+```
+python -m pip install --upgrade pip
+```
+
+Install the tools build, twine and bumpver: 
+```
+python -m pip install build twine bumpver
+```
+Upgrade the setuptools: 
+
+```
+pip install --upgrade setuptools
+```
+
+Bump the version in pyproject.toml: 
+```
+bumpver update --patch
+```
 This will commit a new version to GitHub.
 
-Build the project: `python -m build`
-
-Check the distribution: `twine check dist/*`
-
-Upload to test-pypi to validate: `twine upload -r testpypi dist/*`
+Build the project: 
+```
+python -m build
+```
+
+Check the distribution: 
+```
+twine check dist/*
+```
+
+Upload to test-pypi to validate: 
+```
+twine upload -r testpypi dist/*
+```
 
 Login with username: svabra (password should be known)
 
-If the test-upload was successful, finally, upload to pypi production: `twine upload dist/*`
+If the test-upload was successful, finally, upload to pypi production: 
+```
+twine upload dist/*
+```
 
 Done.
 
-(P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)
+(P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)bumpver update --patch
```

### Comparing `fa-models-1.0.40/README.md` & `fa-models-1.0.43/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,52 +21,98 @@
 ### Installation as Consuming Developer
 
 Simply run: `pip install fa-models`
 
 Import in modules without the dash (e.g.): `from famodels.signal import Signal`
 
 ### Setup as Contributor
-Create the virtul environment: `py -m venv .venv`
-Start the Environment: `./.venv/Scripts/activate`. Use `deactivate`to stop it.
-Update the PIP: `py -m pip install --upgrade pip`
-
-All the required libraries must be listed in requirements.txt and installed by  `py -m pip install -r .\requirements.txt`
+Create the virtul environment: 
+```
+py -m venv .venv
+```
+Start the Environment: 
+```
+./.venv/Scripts/activate
+```
+ (or allow VS Code to start it). Use `deactivate`to stop it.
+
+All the required libraries must be listed in requirements.txt and installed by  
+```
+python -m pip install -r .\requirements.txt
+```
+For Dev use 
+```
+python -m pip install -r .\requirements-dev.txt
+```
 
 To cleanup the environment run:
-`pip3 freeze > to-uninstall.txt` and then
-`pip3 uninstall -y -r to-uninstall.txt`
-
-or `pip3 install pip-autoremove`
+```
+pip3 freeze > to-uninstall.txt
+```
+ and then
+```
+pip3 uninstall -y -r to-uninstall.txt
+```
+
+or 
+```
+pip3 install pip-autoremove
+```
 
 ### Build Library
 Prerequisite: make sure that you give your Operating System user the right to modify files in the python directory. The directory where pyhton is installed.
 Use `python setup.py bdist_wheel` to create the dist, build and .eggs folder.
 
 ## Reference from a different project
 In order to use your own version of the project - to maybe contribute to the library - simply clone the code from github into new directory. Then add the path of that new directory to the requirements.txt file of your project. Then change in fa-models whatever you recommend to improve. Don't forget the Open-Closed Principle: extend only (unless it requires a breaking change)
 
 
 ### Releasing a new version
 
 Delete any old files in the /dist and build folder of your local environment.
-Update your pip: `python -m pip install --upgrade pip`
-
-Install the tools build, twine and bumpver: `python -m pip install build twine bumpver`
-Upgrade the setuptools: `pip install --upgrade setuptools`
-
-Bump the version in pyproject.toml: `bumpver update --patch`
+Update your pip: 
+```
+python -m pip install --upgrade pip
+```
+
+Install the tools build, twine and bumpver: 
+```
+python -m pip install build twine bumpver
+```
+Upgrade the setuptools: 
+
+```
+pip install --upgrade setuptools
+```
+
+Bump the version in pyproject.toml: 
+```
+bumpver update --patch
+```
 This will commit a new version to GitHub.
 
-Build the project: `python -m build`
-
-Check the distribution: `twine check dist/*`
-
-Upload to test-pypi to validate: `twine upload -r testpypi dist/*`
+Build the project: 
+```
+python -m build
+```
+
+Check the distribution: 
+```
+twine check dist/*
+```
+
+Upload to test-pypi to validate: 
+```
+twine upload -r testpypi dist/*
+```
 
 Login with username: svabra (password should be known)
 
-If the test-upload was successful, finally, upload to pypi production: `twine upload dist/*`
+If the test-upload was successful, finally, upload to pypi production: 
+```
+twine upload dist/*
+```
 
 Done.
 
-(P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)
+(P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)bumpver update --patch
```

### Comparing `fa-models-1.0.40/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.43/fa_models.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.40
+Version: 1.0.43
 Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -34,52 +34,98 @@
 ### Installation as Consuming Developer
 
 Simply run: `pip install fa-models`
 
 Import in modules without the dash (e.g.): `from famodels.signal import Signal`
 
 ### Setup as Contributor
-Create the virtul environment: `py -m venv .venv`
-Start the Environment: `./.venv/Scripts/activate`. Use `deactivate`to stop it.
-Update the PIP: `py -m pip install --upgrade pip`
-
-All the required libraries must be listed in requirements.txt and installed by  `py -m pip install -r .\requirements.txt`
+Create the virtul environment: 
+```
+py -m venv .venv
+```
+Start the Environment: 
+```
+./.venv/Scripts/activate
+```
+ (or allow VS Code to start it). Use `deactivate`to stop it.
+
+All the required libraries must be listed in requirements.txt and installed by  
+```
+python -m pip install -r .\requirements.txt
+```
+For Dev use 
+```
+python -m pip install -r .\requirements-dev.txt
+```
 
 To cleanup the environment run:
-`pip3 freeze > to-uninstall.txt` and then
-`pip3 uninstall -y -r to-uninstall.txt`
-
-or `pip3 install pip-autoremove`
+```
+pip3 freeze > to-uninstall.txt
+```
+ and then
+```
+pip3 uninstall -y -r to-uninstall.txt
+```
+
+or 
+```
+pip3 install pip-autoremove
+```
 
 ### Build Library
 Prerequisite: make sure that you give your Operating System user the right to modify files in the python directory. The directory where pyhton is installed.
 Use `python setup.py bdist_wheel` to create the dist, build and .eggs folder.
 
 ## Reference from a different project
 In order to use your own version of the project - to maybe contribute to the library - simply clone the code from github into new directory. Then add the path of that new directory to the requirements.txt file of your project. Then change in fa-models whatever you recommend to improve. Don't forget the Open-Closed Principle: extend only (unless it requires a breaking change)
 
 
 ### Releasing a new version
 
 Delete any old files in the /dist and build folder of your local environment.
-Update your pip: `python -m pip install --upgrade pip`
-
-Install the tools build, twine and bumpver: `python -m pip install build twine bumpver`
-Upgrade the setuptools: `pip install --upgrade setuptools`
-
-Bump the version in pyproject.toml: `bumpver update --patch`
+Update your pip: 
+```
+python -m pip install --upgrade pip
+```
+
+Install the tools build, twine and bumpver: 
+```
+python -m pip install build twine bumpver
+```
+Upgrade the setuptools: 
+
+```
+pip install --upgrade setuptools
+```
+
+Bump the version in pyproject.toml: 
+```
+bumpver update --patch
+```
 This will commit a new version to GitHub.
 
-Build the project: `python -m build`
-
-Check the distribution: `twine check dist/*`
-
-Upload to test-pypi to validate: `twine upload -r testpypi dist/*`
+Build the project: 
+```
+python -m build
+```
+
+Check the distribution: 
+```
+twine check dist/*
+```
+
+Upload to test-pypi to validate: 
+```
+twine upload -r testpypi dist/*
+```
 
 Login with username: svabra (password should be known)
 
-If the test-upload was successful, finally, upload to pypi production: `twine upload dist/*`
+If the test-upload was successful, finally, upload to pypi production: 
+```
+twine upload dist/*
+```
 
 Done.
 
-(P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)
+(P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)bumpver update --patch
```

### Comparing `fa-models-1.0.40/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.43/fa_models.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 famodels/generators/__init__.py
 famodels/generators/data_generator.py
 famodels/generators/schema_generator.py
 famodels/models/__init__.py
 famodels/models/direction.py
 famodels/models/order.py
 famodels/models/order_type.py
-famodels/models/processed_trading_signal.py
+famodels/models/processed_signal.py
 famodels/models/side.py
 famodels/models/state_of_signal.py
 famodels/models/state_of_trade.py
 famodels/models/trade.py
 famodels/models/trading_signal.py
+famodels/models/virtual_order.py
 tests/test_data_generator.py
 tests/test_processed_trading_signal.py
 tests/test_produce_schemas.py
 tests/test_schema_generator.py
```

### Comparing `fa-models-1.0.40/famodels/generators/data_generator.py` & `fa-models-1.0.43/famodels/generators/data_generator.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.40/famodels/generators/schema_generator.py` & `fa-models-1.0.43/famodels/generators/schema_generator.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.40/famodels/models/state_of_trade.py` & `fa-models-1.0.43/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.40/famodels/models/trade.py` & `fa-models-1.0.43/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.40/famodels/models/trading_signal.py` & `fa-models-1.0.43/famodels/models/trading_signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import datetime
+import os
 from enum import Enum
 from typing import Optional
 from uuid import UUID
-import uuid
-from sqlmodel import Field, SQLModel
 from famodels.models.direction import Direction
 from famodels.models.side import Side
+from redis_om import Migrator
+from redis_om import (Field, JsonModel)
+from redis_om.connections import get_redis_connection
 
-class BaseSignalSQLModel(SQLModel):
-    def __init__(self, **kwargs):
-        self.__config__.table = False
-        super().__init__(**kwargs)
-        self.__config__.table = True
+REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
+print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
-    class Config:
-        validate_assignment = True
-
-class TradingSignal(SQLModel, table=True):
-    """A trading signal represents a suggestion to buy or sell. It is issued by a signal supplier (manually or algorithmically). It must have a correlating id to a trade."""
-    id: Optional[str] = Field(default=None, primary_key=True)
-    """The id is marked optional - because it will be created by either SQL DB or a async method in an event-driven system.
-        If you add an id here, it will be copied to the trade_correlation_id.
-    """
+class TradingSignal(JsonModel):
+    """A trading signal represents a suggestion to buy or sell. It is issued by a signal supplier (manually or algorithmically). It must have a correlating id to a trade."""    
+    provider_id: str = Field(index=True)
+    """The ID of the provider, who emitted the signal."""
+    algo_id: str = Field(index=True)
+    """Provide the id of your algorithm id (you might have more than one algorithm), which is sending a signal. """
     provider_signal_id: Optional[str]
     """You can use this correlation id as your own 'signal id' of your internal system. 
-    Do not mistaken this correlation id with the trade correlation id."""    
-    provider_trade_id: str
+    #Do not mistaken this correlation id with the trade correlation id."""    
+    provider_trade_id: str = Field(index=True)
     """FA Models describes a Trade as a buy and a sell (not soley a buy or a sell). 
-    Every trade is expected to consist of at least one buy order and zero or more sell orders. 
-    Thus, the trade_correlation_id is mandatory. Use this correlation id to link your signals to a trade. All updates provided by the system will hold the trade id."""
-    is_hot_signal: bool = False
-    """By default, every signal is marked as a cold signal. Thus, set to false. That is a paper-trading signal and will only be processed for forward-performance testing. 
-    Hot signals are suggested to be processed by the order engines - provided all other requirements for hot trading are fulfilled."""    
-    algo_id: str
-    """Provide the id of your algorithm id (you might have more than one algorithm), which is sending a signal. """
-    provider_id: str
-    """The ID of the provider, who emitted the signal."""
-    market: str    
-    """The market you want to trade. e.g. TSLA/USD"""
-    exchange: str
+    # Every trade is expected to consist of at least one buy order and zero or more sell orders. 
+    # Thus, the trade_correlation_id is mandatory. Use this correlation id to link your signals to a trade. All updates provided by the system will hold the trade id."""    
+    is_hot_signal: int = Field(default=0, index=True)
+    """By default, every signal is marked as a cold signal. Thus, set to 0. That is a paper-trading signal and will only be processed for forward-performance testing. 
+    Hot signals are suggested to be processed by the order engines - provided all other requirements for hot trading are fulfilled.
+    Set 1 (not true) to this value to suggest a hot trade."""    
+    market: str = Field(index=True)
+    """The market you want to trade. e.g. BTC/USDT"""
+    exchange: str = Field(index=True)
     """The exchange you pulled your data from - or - wish to trade on."""
-    direction: Direction
+    direction: Direction = Field(index=True)
     """Simply LONG or SHORT."""
-    side: Side
+    side: Side = Field(index=True)
     """Simply BUY (open trade) or SELL (close trade)."""
     price: float
     """The price to buy use for the limit-order or limit-stop-order"""
     tp: float
     """Take-profit in absolute price."""
     sl: float
     """Stop-loss in absolute price."""
-    timestamp_of_creation: int
-    """The timestamp in milliseconds when the signal was created by the signal supplier."""
-    timestamp_of_registration: Optional[int]
-    """The timestamp in milliseconds when the signal was entering our interface. This will be overridden."""
     position_size_of_investment: float = 100
     """Percentage of the investment position this algortihm is allowed to trade. Default is 100%, which is 1 position."""  
-    
+    # datatime.datetime would be fully serializable in REDIS. 
+    # https://www.youtube.com/watch?v=ZP2j7bmWfmU
+    timestamp_of_creation: int = Field(index=True)
+    """The timestamp in milliseconds when the signal was created by the signal supplier."""
+    timestamp_of_registration: Optional[int]
+    """The timestamp in milliseconds when the signal was entering our interface. This will be overridden."""    
+
+    class Meta:
+        global_key_prefix="signal-processing"
+        model_key_prefix="raw-signal"
+        database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
+
+Migrator().run()
```

### Comparing `fa-models-1.0.40/pyproject.toml` & `fa-models-1.0.43/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.40"
+version = "1.0.43"
 description = "The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.40"
+current_version = "1.0.43"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.40/setup.py` & `fa-models-1.0.43/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.40/tests/test_processed_trading_signal.py` & `fa-models-1.0.43/tests/test_processed_trading_signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 
 from time import time
 import pytest
 from famodels.models.direction import Direction
-from famodels.models.processed_trading_signal import ProcessedTradingSignal
+from models.processed_signal import ProcessedTradingSignal
 from famodels.models.side import Side
 from famodels.models.state_of_signal import StateOfSignal
 
 from famodels.models.trading_signal import TradingSignal
 
-SIGNAL_1 = TradingSignal(id="10", provider_signal_id="sifwi", provider_trade_id="wuwor232", is_hot_signal=False, algo_id="232424", market="BTC/USDT", exchange="binance", direction=Direction.LONG, side=Side.BUY, price=20000, tp=22000, sl=19000, timestamp_of_creation=int(time()*1000) )
-SIGNAL_2 = TradingSignal(id="10", provider_signal_id="sifwi", provider_trade_id="wuwor232", is_hot_signal=False, algo_id="232424", market="BTC/USDT", exchange="binance", direction=Direction.LONG, side=Side.BUY, price=20000, tp=22000, sl=19000, timestamp_of_creation=int(time()*1000) )
+SIGNAL_1 = TradingSignal(id="10", provider_signal_id="sifwi", provider_trade_id="wuwor232", is_hot_signal=False, algo_id="232424", market="BTC/USDT", 
+                         exchange="binance", direction=Direction.LONG, side=Side.BUY, price=20000, tp=22000, sl=19000, timestamp_of_creation=int(time()*1000), timestamp_of_registration=int(time()*1000))
+SIGNAL_2 = TradingSignal(id="10", provider_signal_id="sifwi", provider_trade_id="wuwor232", is_hot_signal=False, algo_id="232424", market="BTC/USDT", 
+                         exchange="binance", direction=Direction.LONG, side=Side.BUY, price=20000, tp=22000, sl=19000, timestamp_of_creation=int(time()*1000) )
 
 @pytest.mark.parametrize("signal, invalidations, expectation", [
     (SIGNAL_1, ["Failed to do something smart.", "And also this"] ,True),
     (SIGNAL_2, [], True)
 ])
 def test_instantiation(signal:TradingSignal, invalidations, expectation):
     proc_signal = ProcessedTradingSignal(status=StateOfSignal.ACCEPTED, process_info=[], **signal.__dict__)
```

### Comparing `fa-models-1.0.40/tests/test_produce_schemas.py` & `fa-models-1.0.43/tests/test_produce_schemas.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.40/tests/test_schema_generator.py` & `fa-models-1.0.43/tests/test_schema_generator.py`

 * *Files identical despite different names*

