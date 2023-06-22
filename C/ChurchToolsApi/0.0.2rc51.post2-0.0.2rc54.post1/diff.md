# Comparing `tmp/churchtoolsapi-0.0.2rc51.post2.tar.gz` & `tmp/churchtoolsapi-0.0.2rc54.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "churchtoolsapi-0.0.2rc51.post2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "churchtoolsapi-0.0.2rc54.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `churchtoolsapi-0.0.2rc51.post2.tar` & `churchtoolsapi-0.0.2rc54.post1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      340 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1252 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       10 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/CODEOWNERS
--rw-r--r--   0        0        0      417 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/dependabot.yml
--rw-r--r--   0        0        0      245 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/issue-branch.yml
--rw-r--r--   0        0        0      418 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/template-sync.yml
--rw-r--r--   0        0        0     1252 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.gitignore
--rw-r--r--   0        0        0     1540 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.pypirc
--rw-r--r--   0        0        0      458 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.vscode/launch.json
--rw-r--r--   0        0        0      875 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/.vscode/settings.json
--rw-r--r--   0        0        0      444 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1146 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/LICENSE
--rw-r--r--   0        0        0    14946 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/README.md
--rw-r--r--   0        0        0     2780 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/SECURITY.md
--rw-r--r--   0        0        0     1308 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/SUPPORT.md
--rw-r--r--   0        0        0      634 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/Makefile
--rw-r--r--   0        0        0     2356 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/conf.py
--rw-r--r--   0        0        0      359 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/developer.md
--rw-r--r--   0        0        0      468 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/make.bat
--rw-r--r--   0        0        0       57 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/modules.rst
--rw-r--r--   0        0        0      471 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16089 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/pyproject.md
--rw-r--r--   0        0        0      437 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      427 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/python_package.rst
--rw-r--r--   0        0        0       42 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/requirements.txt
--rw-r--r--   0        0        0       44 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/vscode.md
--rw-r--r--   0        0        0      208 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/docs/workflows.md
--rw-r--r--   0        0        0     6885 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/pyproject.toml
--rw-r--r--   0        0        0      396 2023-06-21 23:30:32.885059 churchtoolsapi-0.0.2rc51.post2/src/ChurchToolsApi/__init__.py
--rw-r--r--   0        0        0     5005 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/src/ChurchToolsApi/churchtools_api.py
--rw-r--r--   0        0        0     1307 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/src/ChurchToolsApi/exceptions.py
--rw-r--r--   0        0        0       43 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/src/README.md
--rw-r--r--   0        0        0     2445 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/tests/conftest.py
--rw-r--r--   0        0        0     2595 2023-06-21 23:30:15.880915 churchtoolsapi-0.0.2rc51.post2/tests/test_churchtools_api.py
--rw-r--r--   0        0        0    16877 1970-01-01 00:00:00.000000 churchtoolsapi-0.0.2rc51.post2/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1252 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       10 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      417 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      245 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/issue-branch.yml
+-rw-r--r--   0        0        0      418 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0     1252 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.pypirc
+-rw-r--r--   0        0        0      458 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      875 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1146 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/LICENSE
+-rw-r--r--   0        0        0    15656 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/README.md
+-rw-r--r--   0        0        0     2780 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/SUPPORT.md
+-rw-r--r--   0        0        0      634 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/docs/Makefile
+-rw-r--r--   0        0        0     2356 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/docs/conf.py
+-rw-r--r--   0        0        0      359 2023-06-22 00:13:15.968405 churchtoolsapi-0.0.2rc54.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/make.bat
+-rw-r--r--   0        0        0       57 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16089 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      427 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6885 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/pyproject.toml
+-rw-r--r--   0        0        0      396 2023-06-22 00:13:34.669723 churchtoolsapi-0.0.2rc54.post1/src/ChurchToolsApi/__init__.py
+-rw-r--r--   0        0        0     5005 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/src/ChurchToolsApi/churchtools_api.py
+-rw-r--r--   0        0        0     1307 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/src/ChurchToolsApi/exceptions.py
+-rw-r--r--   0        0        0       43 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/src/README.md
+-rw-r--r--   0        0        0     2445 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2595 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/tests/test_churchtools_api.py
+-rw-r--r--   0        0        0      745 2023-06-22 00:13:15.972406 churchtoolsapi-0.0.2rc54.post1/tests/test_integrations.py
+-rw-r--r--   0        0        0    17587 1970-01-01 00:00:00.000000 churchtoolsapi-0.0.2rc54.post1/PKG-INFO
```

### Comparing `churchtoolsapi-0.0.2rc51.post2/.devcontainer/devcontainer.json` & `churchtoolsapi-0.0.2rc54.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/.github/workflows/CI.yml` & `churchtoolsapi-0.0.2rc54.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/.github/workflows/schedule-update-actions.yml` & `churchtoolsapi-0.0.2rc54.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/.gitignore` & `churchtoolsapi-0.0.2rc54.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/.pre-commit-config.yaml` & `churchtoolsapi-0.0.2rc54.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/.vscode/settings.json` & `churchtoolsapi-0.0.2rc54.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/LICENSE` & `churchtoolsapi-0.0.2rc54.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/README.md` & `churchtoolsapi-0.0.2rc54.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -93,7 +93,21 @@
 ## Getting Started
 
 To get started with this template, simply 'Use This Template' to create a new repository and start building your project within the `src` directory. Try to open the project in GitHub Codespace, and to run the unit tests using the VS Code Test extension.
 
 ## Contributing
 
 This project welcomes contributions and suggestions. For details, visit the repository's [Contributor License Agreement (CLA)](https://cla.opensource.microsoft.com) and [Code of Conduct](https://opensource.microsoft.com/codeofconduct/) pages.
+
+
+Available types:
+ - feat: A new feature
+ - fix: A bug fix
+ - docs: Documentation only changes
+ - style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
+ - refactor: A code change that neither fixes a bug nor adds a feature
+ - perf: A code change that improves performance
+ - test: Adding missing tests or correcting existing tests
+ - build: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
+ - ci: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
+ - chore: Other changes that don't modify src or test files
+ - revert: Reverts a previous commit
```

### Comparing `churchtoolsapi-0.0.2rc51.post2/SECURITY.md` & `churchtoolsapi-0.0.2rc54.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/SUPPORT.md` & `churchtoolsapi-0.0.2rc54.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/docs/Makefile` & `churchtoolsapi-0.0.2rc54.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/docs/conf.py` & `churchtoolsapi-0.0.2rc54.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/docs/make.bat` & `churchtoolsapi-0.0.2rc54.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/docs/pylint.md` & `churchtoolsapi-0.0.2rc54.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/pyproject.toml` & `churchtoolsapi-0.0.2rc54.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/src/ChurchToolsApi/churchtools_api.py` & `churchtoolsapi-0.0.2rc54.post1/src/ChurchToolsApi/churchtools_api.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/src/ChurchToolsApi/exceptions.py` & `churchtoolsapi-0.0.2rc54.post1/src/ChurchToolsApi/exceptions.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/tests/conftest.py` & `churchtoolsapi-0.0.2rc54.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/tests/test_churchtools_api.py` & `churchtoolsapi-0.0.2rc54.post1/tests/test_churchtools_api.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc51.post2/PKG-INFO` & `churchtoolsapi-0.0.2rc54.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChurchToolsApi
-Version: 0.0.2rc51.post2
+Version: 0.0.2rc54.post1
 Summary: A Python wrapper for the ChurchTools API
 Author-email: Felix Kotschenreuther <felix.kotschenreuther@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -134,7 +134,21 @@
 
 To get started with this template, simply 'Use This Template' to create a new repository and start building your project within the `src` directory. Try to open the project in GitHub Codespace, and to run the unit tests using the VS Code Test extension.
 
 ## Contributing
 
 This project welcomes contributions and suggestions. For details, visit the repository's [Contributor License Agreement (CLA)](https://cla.opensource.microsoft.com) and [Code of Conduct](https://opensource.microsoft.com/codeofconduct/) pages.
 
+
+Available types:
+ - feat: A new feature
+ - fix: A bug fix
+ - docs: Documentation only changes
+ - style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
+ - refactor: A code change that neither fixes a bug nor adds a feature
+ - perf: A code change that improves performance
+ - test: Adding missing tests or correcting existing tests
+ - build: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
+ - ci: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
+ - chore: Other changes that don't modify src or test files
+ - revert: Reverts a previous commit
+
```

