# Comparing `tmp/django_tailwind-3.5.0.tar.gz` & `tmp/django_tailwind-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind-3.5.0.tar", max compression
+gzip compressed data, was "django_tailwind-3.6.0.tar", max compression
```

## Comparing `django_tailwind-3.5.0.tar` & `django_tailwind-3.6.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1078 2022-06-19 15:34:32.655277 django_tailwind-3.5.0/LICENSE
--rw-r--r--   0        0        0     1513 2022-06-19 15:18:01.203485 django_tailwind-3.5.0/README.md
--rw-r--r--   0        0        0     1286 2023-02-16 23:15:44.823027 django_tailwind-3.5.0/pyproject.toml
--rw-r--r--   0        0        0      524 2022-06-19 18:45:11.070325 django_tailwind-3.5.0/src/tailwind/__init__.py
--rw-r--r--   0        0        0       80 2022-06-19 15:17:54.342526 django_tailwind-3.5.0/src/tailwind/app_template/cookiecutter.json
--rw-r--r--   0        0        0      292 2023-02-16 23:06:00.319924 django_tailwind-3.5.0/src/tailwind/app_template/hooks/pre_gen_project.py
--rw-r--r--   0        0        0        0 2022-06-19 15:17:54.342695 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/__init__.py
--rw-r--r--   0        0        0      169 2022-06-19 15:17:54.344128 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/apps.py
--rw-r--r--   0        0        0       13 2022-06-19 15:34:32.631654 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/.gitignore
--rw-r--r--   0        0        0     1021 2023-02-16 22:19:10.262877 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/package.json
--rw-r--r--   0        0        0      121 2022-06-19 15:17:54.345072 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/postcss.config.js
--rw-r--r--   0        0        0       59 2022-06-19 15:17:54.345274 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/src/styles.css
--rw-r--r--   0        0        0     1935 2022-06-19 15:34:32.756250 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/tailwind.config.js
--rw-r--r--   0        0        0      556 2022-06-19 15:17:54.345754 django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/templates/base.html
--rw-r--r--   0        0        0       91 2022-06-19 15:17:54.346694 django_tailwind-3.5.0/src/tailwind/apps.py
--rw-r--r--   0        0        0        0 2022-06-19 15:17:54.346794 django_tailwind-3.5.0/src/tailwind/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-19 15:17:54.346886 django_tailwind-3.5.0/src/tailwind/management/commands/__init__.py
--rw-r--r--   0        0        0     4121 2022-06-19 18:59:17.999429 django_tailwind-3.5.0/src/tailwind/management/commands/tailwind.py
--rw-r--r--   0        0        0     1150 2022-06-19 19:02:38.611508 django_tailwind-3.5.0/src/tailwind/npm.py
--rw-r--r--   0        0        0      494 2022-06-19 15:17:54.349663 django_tailwind-3.5.0/src/tailwind/templates/tailwind/tags/css.html
--rw-r--r--   0        0        0      187 2022-06-19 15:17:54.350498 django_tailwind-3.5.0/src/tailwind/templates/tailwind/tags/preload_css.html
--rw-r--r--   0        0        0      711 2022-06-19 15:17:54.350985 django_tailwind-3.5.0/src/tailwind/templatetags/tailwind_tags.py
--rw-r--r--   0        0        0      762 2023-02-16 23:09:30.440206 django_tailwind-3.5.0/src/tailwind/utils.py
--rw-r--r--   0        0        0     1018 2022-06-19 15:38:10.139165 django_tailwind-3.5.0/src/tailwind/validate.py
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 django_tailwind-3.5.0/setup.py
--rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 django_tailwind-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-22 19:15:57.935857 django_tailwind-3.6.0/LICENSE
+-rw-r--r--   0        0        0     1387 2023-06-22 19:15:57.936009 django_tailwind-3.6.0/README.md
+-rw-r--r--   0        0        0     1372 2023-06-22 19:55:28.964769 django_tailwind-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0      524 2023-06-22 19:15:57.949252 django_tailwind-3.6.0/src/tailwind/__init__.py
+-rw-r--r--   0        0        0       80 2023-06-22 19:15:57.949343 django_tailwind-3.6.0/src/tailwind/app_template/cookiecutter.json
+-rw-r--r--   0        0        0      292 2023-06-22 19:15:57.949439 django_tailwind-3.6.0/src/tailwind/app_template/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:15:57.949498 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-22 19:15:57.949574 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/apps.py
+-rw-r--r--   0        0        0       13 2023-06-22 19:15:57.949674 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/.gitignore
+-rw-r--r--   0        0        0     1021 2023-06-22 19:20:12.235781 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/package.json
+-rw-r--r--   0        0        0      121 2023-06-22 19:15:57.949788 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-06-22 19:15:57.949881 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/src/styles.css
+-rw-r--r--   0        0        0     1935 2023-06-22 19:15:57.949952 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/tailwind.config.js
+-rw-r--r--   0        0        0      556 2023-06-22 19:15:57.950043 django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/templates/base.html
+-rw-r--r--   0        0        0       91 2023-06-22 19:15:57.950097 django_tailwind-3.6.0/src/tailwind/apps.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:15:57.950155 django_tailwind-3.6.0/src/tailwind/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:15:57.950230 django_tailwind-3.6.0/src/tailwind/management/commands/__init__.py
+-rw-r--r--   0        0        0     4121 2023-06-22 19:15:57.950332 django_tailwind-3.6.0/src/tailwind/management/commands/tailwind.py
+-rw-r--r--   0        0        0     1150 2023-06-22 19:15:57.950394 django_tailwind-3.6.0/src/tailwind/npm.py
+-rw-r--r--   0        0        0      494 2023-06-22 19:15:57.950554 django_tailwind-3.6.0/src/tailwind/templates/tailwind/tags/css.html
+-rw-r--r--   0        0        0      187 2023-06-22 19:15:57.950618 django_tailwind-3.6.0/src/tailwind/templates/tailwind/tags/preload_css.html
+-rw-r--r--   0        0        0      896 2023-06-22 19:38:06.085440 django_tailwind-3.6.0/src/tailwind/templatetags/tailwind_tags.py
+-rw-r--r--   0        0        0      762 2023-06-22 19:15:57.950771 django_tailwind-3.6.0/src/tailwind/utils.py
+-rw-r--r--   0        0        0     1018 2023-06-22 19:15:57.950832 django_tailwind-3.6.0/src/tailwind/validate.py
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 django_tailwind-3.6.0/PKG-INFO
```

### Comparing `django_tailwind-3.5.0/LICENSE` & `django_tailwind-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/README.md` & `django_tailwind-3.6.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -24,12 +24,11 @@
 ```bash
 pip install django-tailwind
 ```
 
 Check docs for the [Installation](https://django-tailwind.readthedocs.io/en/latest/installation.html) instructions.
 
 ## Bugs and suggestions
-If you have found a bug, please use the issue tracker on GitHub.
 
-[https://github.com/timonweb/django-tailwind/issues](https://github.com/timonweb/django-tailwind/issues)
+Please see [CONTRIBUTING](CONTRIBUTING.md).
 
 2019 - 2022 (c) [Tim Kamanin - A Full Stack Django Developer](https://timonweb.com)
```

### Comparing `django_tailwind-3.5.0/pyproject.toml` & `django_tailwind-3.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-tailwind"
-version = "3.5.0"
+version = "3.6.0"
 description = "Tailwind CSS Framework for Django projects"
 authors = ["Tim Kamanin <tim@timonweb.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/timonweb/django-tailwind"
 keywords = ["django", "tailwind", "css"]
 classifiers = [
@@ -24,24 +24,27 @@
 packages = [
     { include = "tailwind", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 django = ">=3.2.14"
-django-browser-reload = "^1.6.0"
+django-browser-reload = {version = "^1.6.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-django = "^4.5.2"
 tox = "^4.4.5"
 pre-commit = "^3.0.4"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 Sphinx = "^4.3.1"
 recommonmark = "^0.7.1"
 sphinx-rtd-theme = "^1.2.0"
 
+[tool.poetry.extras]
+reload = ["django-browser-reload"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_tailwind-3.5.0/src/tailwind/__init__.py` & `django_tailwind-3.6.0/src/tailwind/__init__.py`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/tailwind.config.js` & `django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/static_src/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/src/tailwind/app_template/{{cookiecutter.app_name}}/templates/base.html` & `django_tailwind-3.6.0/src/tailwind/app_template/{{cookiecutter.app_name}}/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/src/tailwind/management/commands/tailwind.py` & `django_tailwind-3.6.0/src/tailwind/management/commands/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/src/tailwind/npm.py` & `django_tailwind-3.6.0/src/tailwind/npm.py`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/src/tailwind/utils.py` & `django_tailwind-3.6.0/src/tailwind/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/src/tailwind/validate.py` & `django_tailwind-3.6.0/src/tailwind/validate.py`

 * *Files identical despite different names*

### Comparing `django_tailwind-3.5.0/PKG-INFO` & `django_tailwind-3.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind
-Version: 3.5.0
+Version: 3.6.0
 Summary: Tailwind CSS Framework for Django projects
 Home-page: https://github.com/timonweb/django-tailwind
 License: MIT
 Keywords: django,tailwind,css
 Author: Tim Kamanin
 Author-email: tim@timonweb.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -20,16 +20,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Provides-Extra: reload
 Requires-Dist: django (>=3.2.14)
-Requires-Dist: django-browser-reload (>=1.6.0,<2.0.0)
+Requires-Dist: django-browser-reload (>=1.6.0,<2.0.0) ; extra == "reload"
 Description-Content-Type: text/markdown
 
 # Tailwind CSS integration for Django a.k.a. Django + Tailwind = 💚
 ![Django Tailwind Demo](https://raw.githubusercontent.com/timonweb/django-tailwind/master/docs/django-tailwind-demo-800.gif)
 
 ## Goal
 This project aims to provide a comfortable way of using the *Tailwind CSS* framework within a Django project.
@@ -54,13 +55,12 @@
 ```bash
 pip install django-tailwind
 ```
 
 Check docs for the [Installation](https://django-tailwind.readthedocs.io/en/latest/installation.html) instructions.
 
 ## Bugs and suggestions
-If you have found a bug, please use the issue tracker on GitHub.
 
-[https://github.com/timonweb/django-tailwind/issues](https://github.com/timonweb/django-tailwind/issues)
+Please see [CONTRIBUTING](CONTRIBUTING.md).
 
 2019 - 2022 (c) [Tim Kamanin - A Full Stack Django Developer](https://timonweb.com)
```

